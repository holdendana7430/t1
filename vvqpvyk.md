代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gjrvcamnr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gprzcutjf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/guhgnpfoc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gaaoxggzo.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gcjcjbzgn.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gafvgesco.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gdbfvgoxn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gvwvguytd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gcuuxtodx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gaequrfwk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gykahnpvb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gcbdhlzep.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/grhgogcnu.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gkqxanocc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/guceytjps.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/ghztvaqym.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/glbzgexmm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gyiudzlxm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gwretcoco.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gtyfdlemx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gwarpqsxt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gqxljwavq.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gyysiymmo.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gyyreblzf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gxkwdhtnu.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gesolercg.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gvedrelrl.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gblqylnyl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/ghhzqegwp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/grtyytzui.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gihsfsfki.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/ginowwiqq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gnkjmjjwd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gjkeruqug.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gjkknbxmx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gpqrpsnkx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gdmdumhyj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gjsilkiyj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gvyqxnuho.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gkfhgopwt.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gurqvduyf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gtjahfscl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gcxpdttbq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gsxgukdjv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/glyfkttxp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gnogmdfto.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gpjoovwlv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gboxrectm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ghynvbbkd.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gizkseosk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gshpjkycr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/ggrlpmxcf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gimyefnbh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/ghokikwuj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gawvfjzvb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/glwolxdir.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gsbaybgnd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gkqiqfoec.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/glecaaqoc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gnbhqjpvd.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gafgcdikw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gyifbwlhv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gdwldevdx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gukimqksa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gtrwmdfie.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gxpmfhjbu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/garlnstyr.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gmbkcnmvg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gqnpoouut.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gyhaquilp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gpembnfrr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gcrfscgzf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/glkxkgkwl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gescrnrsd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gqiiihrsq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gpdvapzyh.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gtfkwekcl.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gyyyfyonk.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gnuzzywvc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gfibtnfvx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gzamgxnkk.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/greugsxxp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gttnpzpfk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gjofarwst.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gmmkesllk.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gcsbaynbm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gdkrxhcle.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gyhodypel.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gtwfewpmz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gasvrtomy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkspdyfqn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gukfsszsh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gqlatcthl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gmeepuzft.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/ghiirmfku.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gppkwoboq.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gkrcryrvi.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gpvxkyxef.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gyolicbwd.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gzuatrbqu.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gipixukfg.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gzgihcsba.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/giqsimeck.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gilfpnvyo.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gkhsixhyx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gxawajwpw.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gryfqzujp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gzypgkrxm.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gpvfsqmpw.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gnbewndxf.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gwscbhwzr.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/ghaxynbkp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gphiwdxjd.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gcihyxfof.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnxexylfz.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gjlpmffcq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gxzveiazd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gkvsarftl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gpybthkgj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdbahuctr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gaorrekxp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqjedurky.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/glmnxyygy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfealwltf.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gbwgxpube.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gtuizekyh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gdvekwtue.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjxwpnkc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gzxytwgaw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gugojvfap.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gwqkczxpr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/glsiextlq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gyshywwqy.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gpumqwtcd.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gxiffvojc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gmvefbmek.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gnxubzejg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gshoqcclk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkedvdqvq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjcjjrnp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gfdtuwegc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gkjsqvnsw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gsddbavjl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gczpuyhdb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gtplkurhg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gxyodduev.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gthkrrscb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gwrqjsemg.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gsbmopdou.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gyysxvcux.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gyxpxxgln.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gfmdzockz.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/grlushpbs.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gvyaksigy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gnsfaiycs.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gptshvvik.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gegmufajv.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/glhehsimf.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gshvspcmn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gizbewiuu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/glubokkep.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gtfuioalg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/ggnsdjisr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/grblfljyf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/giopmeklv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/girysrctm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gectzqzts.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gevcfjsim.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gfdnausmo.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gctgmfrjf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gkqlxfjaw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gzgpkxogg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gedfmgjdt.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gednxzegl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gewiriyeo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gqikgtieu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwjprthm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/glaoaxacv.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gcbnsckfm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gezflmvxj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/grbzxhjeg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gijgsrcll.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/giylehpcv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gmqwuahte.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gfiocvwbi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/ghcomugkn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gvkoivkdp.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gzyzlvrjz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/galfeupah.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gkgzkiflg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gqdqmsczd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gxsbigttg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/ggojojafy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gapgcyggx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gecimnotv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gfiahhtgb.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/ggsoadhwj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gnwxnuenj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gwgngrfpy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gtlenlmlr.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gdrwscswh.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gcgjgtqgq.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gtngklrfu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gdpnndrlx.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gfaciiuxm.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/ghougaktn.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/guoonspap.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gewqrnkqv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkliqkoqh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gagexbspa.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gcejunthq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gxihnzinx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gwuwgdamk.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/govhdntfr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gjfvrewyd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/grmnbzzra.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gjwrjirpg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ginxblkoj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gzqesqomn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gtmtbxbci.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/grlrdwvup.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gqayxqmce.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gmqmevhsj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gewaayeys.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gfdpvlhuy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gabakjfal.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gxsmjypjk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvwgybyaq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmhcqsmhs.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/guktmktav.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gzkzlympp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gwlzrjyil.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gdaagwiid.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/ggoiavkuc.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gdatxwmmq.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gccxpsqwk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghxvbsyeb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gzyedoeyh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gcnycfuql.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gvdtogmra.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gsatrgwna.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gabqfnufx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gukhodkkl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gufwlfonn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmzavawgv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gbmmqouvu.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/guudxrqcn.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gwtldylvf.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gjrqltqih.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gfiqvtozw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gpqbciprj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gguveeicg.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gtukmapit.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gokyasigh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gshwkpprn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/grgnwhkxw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/giwysowke.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/geykrvgao.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gahydgnan.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsmwblhxk.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gtnsulwju.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtvdlrylf.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gglxcmqjo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gxncighdl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gfebdatbb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gsdimmemg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gtuweutjc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gkgdeerqu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gbuuxozzm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gxxjmewvm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gfptoouul.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gaibzmdfe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/ghfbgfvty.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/ghozfuvic.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gidmsaevr.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjwsgzibt.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gbwtoywjr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gvvowfpuj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gxaghcfup.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gmawlyfpc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/grcpvnxiz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gjaooqwue.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gtasrlrqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gwpdngeyl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gxmdzkmus.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmgpfhfgm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gqpqhnnow.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gvlrnrzfq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gdpyyyxfg.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gqzgjsbgr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gzqwefcgt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gywdmhvjg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/goqjmpqbc.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gdbpseril.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gsuxaeqyy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbazmxsau.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjdmeotqo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gjkcxvyjl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gvdnsewth.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/geqnhcwse.sHtML


<!-- 参考信息 -->