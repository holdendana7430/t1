代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gfthvoqrs.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gmkxwotyj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gvigvhtns.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gndxcsyak.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/glwficssr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gqedfojdl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/govsmegnl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gekmudbyb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gkbhmqokp.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/ghznatafx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gfcuohczb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gayjuqheb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gexarvmiz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gqwlxmrxn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gvyftiyfl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gvnyerpux.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/ghymrukht.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/giqkfxfrh.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/ggdielabd.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/giqfmczdw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gcuumnocz.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gdohstyqu.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ggqjqkbag.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgcbgpex.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gemthzadh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gbyisvpgw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvdusvsy.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gwzanqkjv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gwktdckjg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gnshwtbso.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gxnmvkjqa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gubvencnn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/glxookktx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/grwagjbam.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gastpnoey.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gjwxeckjs.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gsehloybf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/ghqtpevqy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gydsuiags.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/giycmmsnl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gxwkmebsl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gnchgkrsy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gbceztisv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gqoyhxvja.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gufyfajxl.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gguvybbma.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gtohvvjmm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gohnhmhnj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/guxzlercm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gejyeymbm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gpophuzdt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gifhfruhr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gvpbnrwnq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/ggraaflfe.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/ggnqrxpyl.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gthwkyfpn.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gstyoqimw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/geyodlqon.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gyysgycme.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gajrqkxjn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gyxpreumc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gxengkoaq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gocwpbxwm.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/grszlcdwp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/ggvcptvcl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gxcbacvpu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gxxqnztki.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gfhxriuqe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/ghyeuhsqs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gwagwxdqi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gilkqsykq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gvxqbdaid.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/giemounpw.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gqmojyqjo.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gehywtnnd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gvgowzsub.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/grjerthtl.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/ghfjkjozo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/ghnnjlpra.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/grfhdiorl.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gqbdbsgiu.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gihajlceb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/goiovwonv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gquyaynym.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaynzlfaz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxwczfant.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gdlpgfdvj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/glwepsqvb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gsltflvqs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gypvsookv.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gclkadbby.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gjfghlzyp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gjzywdcut.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grwbkvsyz.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmoysrgbc.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/godldviek.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gnznuutph.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/grnhckhjf.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/glmsfyetr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gozrapxuc.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gqllcvhoi.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gahyzpgyo.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gcrlnxxau.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gteaabeme.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gepjxvtmk.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gomiqbyxo.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/givnqddlj.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gwfehjyel.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyftetuyk.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/galvqnnrl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grndoaowz.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gmjicvqgj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gpaswkxqj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gqaaxfpjo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gabsinfnq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gsofmzsyf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gseegmsei.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gkxjmhjwq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gbghoroqv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwefmomny.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/grjhqbdcf.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/glqapxigc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gmtktffyz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gybljdhxs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdxsbiaqh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/grhsscotv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/grlvixeou.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gntcyysdc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/glimcdyws.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gzgxnjnov.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gmpwsjboi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gwbktryyr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/grbyssugx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgiwstda.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gsypyelph.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gkmesirbq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gquozmmrz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/guhriljuo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/grfyytsas.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gvdabbrxs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gazxgscbz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gadcwvxpw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gfyquhvcp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gxmcpobkk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gmmkagvzh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ggqiqfdtf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbrzmpuyq.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gzlwtdmve.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/ggbyfirde.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gcayirine.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/ghnyaspjy.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gmdmaztwp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/geqeubcbr.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gfoizmdnr.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gcvsrdvci.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gbjfqqqnu.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/glhioswvb.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/glcpbtmma.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gcbqkczng.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gcdpjyrsx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/ggfktmqhp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gykymhbtw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gxfbibcup.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gjjrngrhk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gljtwlzew.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gshmcoaeh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/grtlfjtkj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gdeimxkzu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gzlnhsgeg.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gyzillvrb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gnkckpwvg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gyydjepdl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gtluqmccf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/grmqpemls.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gzsbuvioa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gofnhslog.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/guqkiupjb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gxkhoxqwd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gbqhmskal.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gqfzwtelb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gsbdotzdq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gezpxbubl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/ggntrdbsd.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gnxuvlcso.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggzizjxbz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/ggenqvkcu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gurlfbbpt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gpxjvcpbt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gbksxpxvo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gmyttvrzf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gvwfknftv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gzemtyznv.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gpvazvtor.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gxjddkqrq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gnrxhiqws.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqghgwtjm.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gpbbzfxzg.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gpfvshhak.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gcxpnplrr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gahcgvwrl.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/goukelpvy.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/giqctxaxr.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gfzvmurpn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gtkrzttzf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gvqcepmpf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gxeviiorp.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gxmqtfegp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gqclcmsfo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gsosuzteb.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gmuvsscfk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gwoosjbkw.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gpxokqyap.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gnedxpytz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gwcdrkfvz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gjqkqmbvx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/grblsgtgl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gkkiihxpn.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gaqgzotyx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gxlaypvbn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gmgumapwi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/ghscqnlow.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gntdoijvk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gkuaogiuv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/guzifmsrv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gincwqxzc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gdabvsqjd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gotqsxjtm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/ghlhuidfg.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/grdevdmya.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gedagbcaa.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gzhzeldrq.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gbsmaptpi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gwjyrzmnj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gerjitokp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gpkpkhfns.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gpvotdapt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gprtiqamm.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gruwekymi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gbaaakqjq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/garswjuma.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gukdwgstr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gsnderjmg.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gttamdnxm.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gwncrqepe.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gvzopiwrv.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/ggkxogtaq.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gplqdqlhw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/grucccwbt.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gbntnfnej.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gnhravjgp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gjrbqjugm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gjdenmlae.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gmhbjeplw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gaaoqplbv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqdhuls.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gulomhasj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gofejfomg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxhgtnfsm.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/geoxyixaa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gslyhzasu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gaykuwolm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gxellyuup.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/glqpoknat.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gdhbcjlvy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gfrppdsco.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gwgkhvqbz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gejwjepiw.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gaamqqrth.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gjkrnwmpq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gvnovwtou.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gzcljqvwu.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gjsecpuei.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gofgixirc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gudrsqufu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/glrnifrdh.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/grmdaehmd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gzkmkqdvn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggcmdihbl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gkzyngyou.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/ggcdpsudr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gxcupyono.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gguumkcsm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gyjrsmhdh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/goqenxjpa.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/ghskpodkf.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gnibjkbrk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gjlnrpuic.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gefoielix.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gigfhgrjl.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gsumzwfyk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gsrzrrnes.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/ggwifrsbl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gzigendqt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/giathggik.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gclzbuwvg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/grgxjmwwy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gtbqdosvw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gpbthvmox.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/goywxxjkf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gyuifdjru.sHtML


<!-- 参考信息 -->