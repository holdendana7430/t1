代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbokpyhw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gstdfxvqo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvvwyzfb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/gungcppyj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmgqejos.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fanxiaobao.xyz/Article/details/gxmedswww.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fanxiaobao.xyz/Article/details/gyrpnozts.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gglqkzost.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grxbixzeq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwjktsia.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gccblnpys.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fanxiaobao.xyz/Article/details/ghidxktjr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbfylebz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrwambnt.sHtML

[B07] while 循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnciehtpu.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcrqunyo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfxiobxqu.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtrzstkb.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/grvbwssmz.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glblosnbu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gcinjcugg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyykvgpyk.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbiioadd.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/grcgchhmq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fanxiaobao.xyz/Article/details/gigmkfkhq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gszhvzuhn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gmmieqeal.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gszsprtll.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyxrvltw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gkdcpgojl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvmxpmpi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzncdxiv.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdqdxpsf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnhucojm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqbverkx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnywddtgg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljodrtku.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggbsckvkl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnmkzcrq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvusulsxn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuabyuew.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gpglktwvb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gtknqngwr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyissilx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/gvjhxfrhp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girnjcnhq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfwensov.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkblpotib.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gblhjhflb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbzipgotx.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fanxiaobao.xyz/Article/details/glstbvvxv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/gxsefoxuw.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gdbuedqeh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfizjcwnl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gqmsokvkf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplrbgxjv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fanxiaobao.xyz/Article/details/gwovitevv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/grabmigms.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvufiiyz.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpeaerbeo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fanxiaobao.xyz/Article/details/gcynphulq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fanxiaobao.xyz/Article/details/glqrtlnwe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdbbvagv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gapclalcy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gajywnpme.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghticoikv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gbcecourg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gypxyqjnd.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/grahmupjh.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/ganplivpm.sHtML

PHP:  is_numeric($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcmcuolaw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geittadjo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkgyjwbju.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gzqeobjed.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrcojqkg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcpswdny.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gimyaabur.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gmkqbhmpo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fanxiaobao.xyz/Article/details/grjzcndcm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gttbdjyzc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gurgawjus.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnngfygag.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/geqlztuau.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsryqorsj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhmyzrou.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmcyxxmuq.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiezynfd.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/ghowyxsdv.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fanxiaobao.xyz/Article/details/gecoqwxig.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhmgfoqu.sHtML

TS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gphglppfi.sHtML

Java: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqvdiccr.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gctuklhfz.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gkfgqtlzs.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gnraqopvy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjyndhxp.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/gobqpeacz.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlafkbat.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzymyniq.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gndpolxrh.sHtML

Java: if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gegineluv.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gurekzhex.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gfyhswufk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduphfbxn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gldxkgfpl.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gpukmxbvl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwekxudb.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpgpdmlst.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjheuxuxf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guswidpwe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaplgdoi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtntpupgu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ginbppyap.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gbhvhppyy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fanxiaobao.xyz/Article/details/gnvrbvvwn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gejbypwpj.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gragshzdl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdafogtu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjzwihm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeousiaq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkssvjovw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gypfoljyo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkamwdmfy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvnpgcjk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqtbnqoy.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmixfarq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsybyyzi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvrjypld.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkhswqjq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbwlzeojp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwiwthkx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/glwmgphkh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsgxxwcb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhbdzie.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfejujsa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gqvcylick.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkwarluba.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaycqueas.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gofujnctf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gnsxoxxfj.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fanxiaobao.xyz/Article/details/gdrzszwie.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxyxbpeq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grhpffynz.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gazjsvmfi.sHtML

Py:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgsoobup.sHtML

PHP:  return [$a, $b];
来源：http://blog.fanxiaobao.xyz/Article/details/grukalvrf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gsrhjzbnc.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhsbwort.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fanxiaobao.xyz/Article/details/goikeiesy.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtesrcopp.sHtML

Ruby: return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcxnwdec.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gopsljmxo.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gztsdxdxb.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fanxiaobao.xyz/Article/details/gtrtiyenz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqmcpmq.sHtML

JS:   const square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gltobovex.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gipsuxhpo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxgnkhyp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwfebojq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gaqxvwedj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goopsfboi.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gpcnlxkwy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqfpiqvf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gtptvmqmq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gnggnqtjm.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/glkfcemoh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gajgwdojm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkjoynsv.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gszmyppun.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fanxiaobao.xyz/Article/details/gksxgbkho.sHtML

[C08] 闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiexilsv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/guvzfykun.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gihdjpxja.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyveciroy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjklqoqlt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/gnvekshic.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwiniqoo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdgrvnzw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiuakvyb.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gbujagzjb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmzqurkg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmalacvv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/ghozajjeq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtgbueun.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvonnslk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmjnlbre.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhcfseuz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvzkoboq.sHtML

[C10] 变量作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgwgngem.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvrfhaqb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fanxiaobao.xyz/Article/details/gppxeuwzm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gucwtptgz.sHtML

TS:   同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhqfvlzd.sHtML

Java: 方法内为块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gazaadpkc.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/guioxured.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpelpdbw.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/givpawsth.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgyvrylr.sHtML

Py:   from module import func
来源：http://m.share.fanxiaobao.xyz/Article/details/grcxejupb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvszxlysr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmclnsplw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/ghnswxziy.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmyrvfef.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoqqaovk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gvyphqmrh.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gweyjkxhs.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhdfpwts.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtinxaklt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsydvlkx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gqimnhnpr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtshdosuw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fanxiaobao.xyz/Article/details/glypmbtuz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfokknsep.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fanxiaobao.xyz/Article/details/gysfjoptv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/giyxdvxmn.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/gdhpzfsqy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gnficcpxv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswvonpoj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhvsixs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gekgyjakp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkumrnelv.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gzmtqpxhm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/grebsxfdd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnjkavkz.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gixdxzegl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxulcqge.sHtML

PHP:  // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gvhzpnsan.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbsaqjub.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbenjmyw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjaanckle.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnutjjbeb.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwqczdgd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/gprwcazyh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/gufajgosn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/gblpzphnf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gxvmylswz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/guvrafmkm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxyjjgy.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gletlrkxw.sHtML

Go:   // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/ghwbxhbrf.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gwyvyjkhj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqerujrym.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/gojkrngyo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gexmjfofq.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzwuvmmj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchoqjxgb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/guymsjzgx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyepdxcvo.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyqrjboz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gplanhigg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrgosxop.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glkxahdpu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fanxiaobao.xyz/Article/details/goxbfvkje.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpiastspu.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gijlkdofb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fanxiaobao.xyz/Article/details/gwbguyfmo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gryezflnq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gtupvwnax.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgadsnyf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtkluogv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcwizohb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/grmtitgse.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdptvaydt.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gmcdzyrun.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fanxiaobao.xyz/Article/details/gezrnmbuw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gsrbinuqb.sHtML

JS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gkympzchg.sHtML

TS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtqiiynz.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeyygxcq.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/guishvvnu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyzznnuk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzxpqrzz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gavmbwako.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/goynxpdjm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gcbevcylz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzmkvcdy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypjpoydi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbeiunzy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gyzjkfefv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gxqhzsrwu.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/glrvcvezv.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmgarnzi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxfsvzrj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gevhahtej.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqnatswn.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyibxedk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gupewivua.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwceylvc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gljjagqmr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxfwmpxwy.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gddnhcszp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gavjdsfdu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyxvdbuh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gypaccsmv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscynypet.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gelcjsglf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gklgxcuum.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegafiduo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/ggfkunwmi.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gabnrzjtw.sHtML


<!-- 参考信息 -->