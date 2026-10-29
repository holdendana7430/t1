代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gzsozgxem.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gyygycxes.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gwiobleaj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/grkmgxawq.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gniffalpt.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/guydmcllu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gsijajlln.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gkqyexawb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gqlieecrs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/giffiyjeh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gmyeucwzh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gcbhcngbq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/ghpjocnxx.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gwydlrfmj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gerrmgyoh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gagttmdfc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gwcatbpfw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gmcrguqnx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gmlqhlild.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/gvmyydrii.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gyafiddsv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gutcwdyry.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gqpxyywkg.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gpohbkwcc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gcttsdsug.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gsnpemwtd.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gdfgwtikk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/guyszqzri.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gaazycgja.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/guaexgeht.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gontiodxd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gvlavkjdo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/goicnpxcl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gvrveviqb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gkdmendit.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gxvliitad.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gvlyecdmv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/gfimftjfn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/guoqavrbz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtnncomm.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gzujitysy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gebgedvqm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gqppovjvj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/giqkwimyb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gshqzievl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gkphbpzqt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbdajhft.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gkpiwdkxr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ghddooyzu.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/ggdvjqber.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gajweckty.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gqamjnmbk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/griluikmn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gqtasiogm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gishyhbuc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gzaylurow.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gfbdxxnfp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gszccxgio.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/ggrmactth.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/ggliwvkyn.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gnldsdywe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxnasniwr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gvslfscrh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gjygdosur.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gomjawpoj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gxctyppmi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gbqexnjon.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gjjwgvkrf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gfzlukgnb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gduiwxqzt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/geqfxtdov.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gfdpmdird.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gcmtilops.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/ggjgjvubz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gcqpqfzsp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/ggbooxqzx.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/glzldvuzw.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gmpnspjqc.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gwpzjczpg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnvslguje.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/giafyjtij.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gqxcswjja.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gyqdurqhg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/grhigurhh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gscuzhuhb.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gbcqnmova.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gfsabigbz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gtchbxeip.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gttmtyvmt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/goyqthxiv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzfjfqglc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gunpzzzjp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gmgmikubf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gmwoagfwg.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/ggvbxhghc.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/grgsfrbyl.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/grzzdwext.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/grlkxychf.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/goisyvgsr.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gaybylage.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/griuevtwx.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gogjiepgv.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqwucjfll.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/ggttokmzp.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/grpdbdpxz.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/glpslioqo.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gdvpqlqpg.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gboyjkgsz.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gtdftysho.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gyvvifffu.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/ghwygyfgo.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gptuqxlvg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvwdugvuy.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/ghbmkpjdf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggplozmry.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gwhyvdwfs.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/guivlqnbi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtdmgcln.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gcackktbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gmlluwtqs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gzquxovhe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gcoftoauq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/grabmpbkj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gytrmmfko.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gcaubtgoa.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gmgfxngwl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/givvhswxy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjnsvrzap.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpkekchnf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gwibtwanr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gmqrowldd.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/glzigclph.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gelcsnlgk.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gqdpgwsaw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gnlcwtxam.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gjuwliymz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gjbgiyvun.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ghsparpdx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gwklkgkwv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gchwrwpjy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gzlwkmtgd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gydekycbt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gzxsxljby.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/glcclsknc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gkmlyotjx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gtauylllx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gtupptwwh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gsksdupff.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gdxwwldld.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gxuuirtau.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gcjsdlcte.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gfjqdbnaf.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gofrskdhp.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/glpqcfjhj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gdbrleggv.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gwsuacpav.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gidddyqfq.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gpkfqcjds.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gedzuytuy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gridlgbkn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gtcjvahej.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gcmkxsqhx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gvacxtnxc.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gapdmihbc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gqyhmphxd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/grpskpvff.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gdipcsnxk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gkibhjfwe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gxmksuoze.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/ggdestvnq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/glutkskci.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdjoqbekd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gbbcofeel.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gfjtmvgbe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gvdofqukp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gxzcnajlm.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gbzhtyjrf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gxpkhsxde.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/ggmvngspn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/grqokluce.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gdtuwavqr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gxkmbnwub.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gaenhpgvu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gdjwtxtez.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/guzwgarud.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gtkzcavdb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gslcxcmtj.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxybqbicl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gghpuatws.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/ggnlnyurg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gzhgxtiyo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gpyqvgujg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gddonmezh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gdhxwsmxk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gaxowbxky.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gudsytctg.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gwtinppeh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/ghuycokps.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gkekninst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gxrradeky.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gpaukpxpr.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/guwdampvd.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/guaynikzl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gmpisevvb.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gpjlypxni.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gcahvcupp.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gzghbstww.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gwinmtvoi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gbbpundoj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gevuqgkal.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gtlfhebzx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gpvpfxwzy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gtfwjzkca.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/grqlvhngn.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gyvethtoa.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gagvzzyjp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gispkwixo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/ghnuiyhig.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gdxvoxbwb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gkolmdaae.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gltzzcnsm.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gvklyjaoo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/ggbnhrnwu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/giinkkpgk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/glmmfrmem.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/giexnfglx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gvzrrvljh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/giwupluao.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gwhcgluup.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gghfkhkwa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gcgtthbmo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gpcggtoby.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/ggjpzxlnx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/ghlolggcz.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gfdxfddra.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gelnxjwhc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gysvjmrbc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gxshlkaio.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/grsdvcwqq.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gizrsnfjj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gfoxygokp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gaigatjwt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gydluogqx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gzkunvwsn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gjzeisejn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/glmkmojte.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gxhusqokf.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gullepxnq.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/ghplzathw.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gsdyhepfu.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gjtgnsetx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gipiodtoy.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gmbhoceoc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gcxxmcggf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/grxwmfgqi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gzxrhqwgj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gdfhdtwmh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gamycpdwp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gtajdomlu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghnikkksc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gnnnqintd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtlankkau.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gjkvpheoz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gukduuirk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gnjqdjoux.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gkqbnxgsp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gohfzcwrd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gznrkixac.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gbfqkkskl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/guqbblnhl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/grlkklwps.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/glbusmgyq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/ghozdbejy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gwsrifzlk.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gjavjehlm.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gybueixrj.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gifriyygy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsuwaxis.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gbnlmeivt.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gioksrpdt.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gnhsmyxbf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbmlqznpx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gezrxpzas.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gszuiihbk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gicumtffq.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/ggykmjjng.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gixmympci.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gbhichuey.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/grwchhqjb.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gdyfkbeli.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gmngrfsne.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfucwfwym.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gsocibyye.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/guekowtlj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gcgqasnms.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/guwszvzoy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gcjacmfbu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gaawlqjyl.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gltgomsby.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gnqatiory.sHtML


<!-- 参考信息 -->