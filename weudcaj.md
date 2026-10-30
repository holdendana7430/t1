代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrxfosdr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/gplqwefrn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqgztfzy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fanxiaobao.xyz/Article/details/gekjrsuvt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gwueoqjys.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzojpsirb.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjupgdiq.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvlypnac.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmdfdfac.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gelzbihyn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubwwlapo.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzhdxrfp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fanxiaobao.xyz/Article/details/gfdiwifkb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaygxjvw.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gacljgkyv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gfoctoteg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdiglgcz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdiawra.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gqsmknvyy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gstrlvxsx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzcsiolh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gphjllvbe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgdmmsoe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkeyzwkh.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdsdqwpz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxsuyzbmv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gissuhczb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqkfdlrh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnsfavqnt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhkcaokm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gswsraeal.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gktozmqaw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvyjtcco.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fanxiaobao.xyz/Article/details/gywsrmmne.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkoyfcqz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ganlalowv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuibvyze.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gtkrfeqcq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gyxoleqfa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gtorsoewh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlzzbslc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdoyalqh.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fanxiaobao.xyz/Article/details/glxzctxns.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/grdlnqbva.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/ggnwilhhz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gztfdykii.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbyenjkij.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/glbtmqdew.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdvrqxrn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gtiahktaj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqihgyqe.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfafyipfu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fanxiaobao.xyz/Article/details/ghgyeugak.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/gxpiifcdg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcliixki.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gczwrjtsq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gaqrshhrd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gidnkwakw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gziiqizbs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gfrokrpoj.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcztuitwk.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/gvitkztkm.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giobuawqq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsaxzbng.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbbjwypyp.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwofpttr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxrmazhh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcraizqg.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfmmlbcw.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fanxiaobao.xyz/Article/details/gmmgtbbru.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gycbyyyhp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjialwdkf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkodamlg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ghesvwswq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gvdwsbukf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcgndsvs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/guxjsutyi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/guunxmmgn.sHtML

[B15] 布尔运算与取反
来源：http://3g.fanxiaobao.xyz/Article/details/gjgodsowp.sHtML

Py:   a and b or not c
来源：http://read.share.fanxiaobao.xyz/Article/details/glgbgqfqq.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gazjfilpt.sHtML

JS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabmtjpt.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclgkcyrk.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfffgkwd.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeicdaab.sHtML

Ruby: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrlghllc.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gyajofqcn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gapmhggld.sHtML

Py:   if not data: return
来源：http://baike.fanxiaobao.xyz/Article/details/gnvvnzxtn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqyifbde.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvvbvbff.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipsuaudq.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvyncznx.sHtML

Go:   if data == nil { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gotthrzqd.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gniayihnf.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gbtdociey.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcweaavmo.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gclicbszr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grikowdia.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcvlyhgc.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gctqjdhoc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwafufpjo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmpsxxsi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gapbydsnh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gumsbsrql.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/glufnxwok.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgfbspmi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgdmxxjd.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpczurlni.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fanxiaobao.xyz/Article/details/gonotgvgp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsqrobxay.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvyhispc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/grekrxaat.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/glpeukzqy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/ghhqnyqdv.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzcniwhe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghchqofz.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gsalsizgf.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkvkvyix.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkdgsrbg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwviokyg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdnwulbx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqttszskl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfovdijq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fanxiaobao.xyz/Article/details/gsnfktetl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gzftgdzrw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbwitgne.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjgtqqbm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggojowbct.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/giopawxzy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gifxjihkc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrzcagrh.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fanxiaobao.xyz/Article/details/gogqalbmy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnizmfrgg.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqzoraazj.sHtML

[C05] 返回多个值
来源：http://www.share.fanxiaobao.xyz/Article/details/gicevlvij.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnpoqjpz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiipaxtf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gckwiuxia.sHtML

TS:   return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gymnhpblk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fanxiaobao.xyz/Article/details/gblvxtlxb.sHtML

Go:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gapxtjjwd.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/grtunqfvx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/gltbcpvei.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwizakit.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gtngshsmn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnwsrzvu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsolbxals.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsppvejw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgyrcubw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gouxlzwej.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/glflirjxg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrhgljnr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gsnvtkuem.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gaberfgfh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgcbsgyt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/gefhvwnqs.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwzbphgz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gnpdwegff.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fanxiaobao.xyz/Article/details/gfomgpbao.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gpimtpmvg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/ghbblofcj.sHtML

[C08] 闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gvtuprvne.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxnfixsq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gottqftau.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlhmwpsr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gceexzkwo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhlqecoc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjoqgzge.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbzskhlw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghbcrsjxw.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gwslgxrwd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnqeohfy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gysspfevg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutmgtell.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzngsxtz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtzjcsrm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxkqitee.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gqidledmz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gsfqwergw.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gitfjydkk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbhruhrh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fanxiaobao.xyz/Article/details/gxspijput.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/glxhsbftx.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gkkeyccgm.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgehzcjc.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/ggldblbgl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fanxiaobao.xyz/Article/details/glwdszfad.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gazkqxggd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojbxvjdl.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/gjptoegsa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gttxzqtga.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdljxsab.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/greqakyei.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvhwqvqw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gmxpazylr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/gyeumpcpp.sHtML

C#:   using System.Text;
来源：http://www.share.fanxiaobao.xyz/Article/details/geqznhxae.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzwcfnsl.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gygtazrtq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gphmkpbej.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gwqjagdbp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gehuqbyar.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/gwouhsbyq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/gvwicvgfu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gmztsnqhb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhtubjkz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgblpyst.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/grrvxvfch.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzjezfjrb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqknfvqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhnmapoh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbppiobcu.sHtML

Go:   func add(a, b int) int
来源：http://3g.fanxiaobao.xyz/Article/details/gwnvetfeg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkolcdla.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/glgdpookx.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqomyebfs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/gzitmnuzy.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwywvdrx.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjqrmmee.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/grkqtuesr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gthhikydp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/goptjtyrr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgwgvrzf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkaoetgi.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcojktvmf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gyrosehxr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkfpvnzh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqmitgjwi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtowfsgws.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gffzfmlzd.sHtML

Go:   // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gmybsastl.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gponfvajs.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gvervnxrj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtaaveod.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gpvfvyqly.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvwaegge.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtltjbizb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gwofyryrj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gygnlqqel.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/guugztomv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/gyijkrbjz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwojhwwm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjtzbtli.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gnihjvmib.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdedywont.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gtqepjurg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvjrrsnm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/guznkoywy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhfufmzn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/guuxricqi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fanxiaobao.xyz/Article/details/gznyuqwlx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fanxiaobao.xyz/Article/details/gpuvcbqxh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpurcdue.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fanxiaobao.xyz/Article/details/gavouqzvi.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gjdzqgpel.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fanxiaobao.xyz/Article/details/girmctvir.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyusvqox.sHtML

JS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpmsqfinh.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwvxqewl.sHtML

Java: list.add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuenefnn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnprcvxxv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/grmbobzyf.sHtML

C#:   list.Add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzawmsdzf.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/gjgvtbaau.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgtmbcol.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflztubqi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbwvvabj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gwcidrqlu.sHtML

Java: list.add(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gionmbfoh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyghdpkbb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouchpkjf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcvequfv.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcxdovcj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/geyjhffaz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gzdpkknol.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwfiwvlq.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gutzamkor.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjdqxfax.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyavuzfau.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdndwemy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbxqhfaok.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvvzxjfo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/guvvwajsc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/grnkhghpl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gcybnjiwa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/girfsisqn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/gnvlazows.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/garamgaux.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gmciifykm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqygxfym.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glyycatip.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gogzbkkxj.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gfjvvagxd.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gdycifdwo.sHtML

TS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdoaeccd.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwgwcsln.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gklqsjmxz.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/geuevzixs.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/ggjugaphj.sHtML


<!-- 参考信息 -->