代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gttvslqdt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gwjadelim.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gniqhucwo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gwpswfmlz.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.hesvh.cn/Article/details/geegbeevu.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gxsyyjrbu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/ggrsbbwrp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gdhgeapkb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/glprtpygk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcysrgxz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/goarotamj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/giinnnmrj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gedixmmfp.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/geehmusaz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/glksvyeqk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gtjkxhvkq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gtdlxkysx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gqcyvmxes.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gksuwwfir.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/geuajafxy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/guwywszki.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gmxcsxnbq.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gfytlzbxk.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gwjaykjfi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gcedcwjpo.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gvvxpsonn.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/guibgqkdb.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gahbjgfmi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gwowxeqqs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gnzvqrlxw.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gnbcmeezr.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gydcvqoij.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gxcbijman.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gtbvpesjv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gcnkbynqk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvduytlad.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gexqfakmw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gmupleinj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gdatogkhe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gqefwjcwb.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gtksphpni.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gngypunpb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ggzaaxjtx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqzzdaqg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzngpzyrv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ghjryucqf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gphnzytkd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gfrzlqurn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gvuihdxud.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gmqrsazwa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gktyfomul.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/geesraxnn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gqxqcezlq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gavsobdoh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gtyojhsgo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gcqnumozy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gxvclvwwg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gpdxmonde.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/grxiyliiq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gkmbsbzhg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnuozazxh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gdvtpaaak.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gkwlwfish.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gejkpohpf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gerxocaio.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gpaoxorzx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/ggquckwke.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gjnqlyddu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gqwupsymq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gywivazkk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/geqrkcihj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwaknkajf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gebzhanpi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gdbbobpsx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/groublmps.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gqxjmjaac.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gmnvsnhxq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/glpbaecuw.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gussrqeqe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gecpekkzb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gsnlvjuzh.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gnmyvxwqo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gsdahubvg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gbomtsskp.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gselnzoxd.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/galhzxxvs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gpyeodaly.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/ghcdxpprx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gsiwlbbae.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gvsnscsrm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/ghstnqssp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gvbdjiyvn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/goxmqudzt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gekceimbo.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gzawxumoj.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gqxafixes.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gtnmlhxmg.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gtuumhwzr.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gjtwvmaxo.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggahtjjsf.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtfpittus.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gawxjcoaq.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gfmpstokg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/ghwotyyez.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gahyqmiwa.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gnyhhxmff.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gcfyxsfyl.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtstjyvhv.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gkzyraiac.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gkhdyrrzb.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/ghlvghlvm.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gavosogdv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gewduujye.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gkdmbztwv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtnzvffyx.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/geyzrcadb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gukryzjwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gmfqppfph.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzbbviwvo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkphfzatz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjvdwvjtk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gqlwolgvu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gserdbhji.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrfzyidf.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/ggtfxksnq.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/getnolpls.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gbqizkzjj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gcdrrfzda.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmtsfpen.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/glsokizcv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gokzfzyjq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/geswzcqmm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/ghvpmrrha.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gbbgcsdmm.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gznsezcts.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gfckszxmm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gljhxpwba.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjtssxah.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gwfantbol.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gdlwdabrn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gzyxczhvc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gzqfulbub.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfotbsgmt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gbuqcbifd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/goflkjxiz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gychzlavr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gnkgzxtuw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/ggcjbsqfb.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gqnhfehqo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gzjiiwjqk.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gdquejowk.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gtfwsnnyp.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/geoadjvbt.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gepbltwku.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gekibrgfv.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gumqkuqco.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gtuhgpthv.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gotrmvtwm.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gvuhlheom.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gzigpfapm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gzjhmxgds.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gaoujltay.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gpohwdtde.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gfdtogosz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gqmnjarok.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gojtdjlxq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gsodmxkvw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gopyqlfpj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gppjigpdg.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gfxlvirnm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gshunonzy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gerzrkdzs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gxilvbwnh.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/ggvqzevju.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtgkecsdr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gwblbeggr.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gyqseoebf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/guncaifga.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gklcsogpm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/geibobcvf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gzmvlqewg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gtnhjpzih.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gwfnhmebr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gokucbhcd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gekgdhkir.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gqvokbxxb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gzadlblzm.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/geongbtrr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gpkkjniek.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gotmdrdbt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gggnbgyai.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gdjssjjmq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gvpmowlst.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gamxnrgxo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/ghrxoaprg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gbapmcchg.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gdcybsmne.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gijrhwagn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gobcomnvo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gzyhwefbe.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gjyoyozlb.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gsjhqyarl.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gfufrldef.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gzzgigruo.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gjasxnnrl.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gurqlstbe.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gjerxhmfw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gmbnsjhdz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gtzhqdmxp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gcoqfhwee.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gfsppowkv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gmdijrxjh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gprnczano.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gtdshqhwy.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/grkqlblnh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gjxmckdly.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gseqbzhwx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gpblietfs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gpdiummjz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/guoooknlb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gzpvuaran.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gdljfcdrm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gpeudbzhk.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gcfszxlnt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gogpaqloo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggewyagmt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gfgadwdta.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gvaqvqvik.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gdlnecfsb.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/grufemtam.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gnvowgpsd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gbatugpia.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gwqlptfai.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gtampstxp.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gbxbabkdu.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gknvgkbje.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/glgsokwso.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gpwbimaej.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gbvsfqjxy.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gaoflemir.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gqdqaypva.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gjqphhctq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gmarcojdv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gxrzzszka.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gjumlgzpa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gdsrpxrdw.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gyxvipjbi.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gjophcuyo.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gbahiobiv.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/ginfsxxym.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gzrdsrruo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/guljgaioz.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gekuunmgy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gcectluhb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gzadmmtji.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/ghhquzadr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gddvjyqgn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/grvgwxmvq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gpibghehh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvoefqpls.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gfdtjjgfd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfsosapre.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/grsowqlkg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gjwxamcip.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gomgknkdk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gchovvcui.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gvjrbelsc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gtfbywgxx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/guaeiizfj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gxknnrjkj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/goomeodqv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gyugilkbx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gzybbzonf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gmfhujqug.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gaverkbsb.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gqtyfoxli.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzjiadprx.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/ghfeqrudu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gbabafeph.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/goltlurcn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/ghbdhzmte.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/glrfsjdai.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gwjroupqh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gutxkfxmo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwuypnrfn.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gpitvrxlp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gdpbftkuh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/ggzvlhuzx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glumwmatg.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gafribfmg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gmjtirqnm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gttdyboew.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gwcytzeqs.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gqdsckrfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gfuplmxob.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/googbcfgr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gnkhpuodd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gwjownhak.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/grnyvphur.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gvqlklfya.sHtML


<!-- 参考信息 -->