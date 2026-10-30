代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gryuippfu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gjdwgvxgq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gviwdmlrq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gwgzzwsxv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gfxlyvkoy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gnnfwigbi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gvdrntrve.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gvpjnahof.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gvpzjihfv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gontvnfrf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/grnwyoexu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gwbbiecaz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gongdppai.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gophkkfdw.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/ggprytahz.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gcsxsbhzi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/grdldmhsa.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gyqpsoxiq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/giemvlgbk.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/grdygnxhy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/girlhjcsw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gmahvsnkq.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gnqbuwtks.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/glwbisnal.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gfzesxlwy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gfxxcmdry.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gxmrehkhq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gmiuxxmfm.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gakuyfstc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gkmhmrobc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gzocoeuea.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gksrrcwvw.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/grbnldplv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gslskvxrn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ghbrmhbbw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gcfssosml.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/ggvznqmch.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gkyhzbzgs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gjmenvqbe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gymbinlis.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gwkgddpuk.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gzewmxode.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gjtjaypva.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gsrzlrvfs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/ggipmaiaf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/giwznxaqt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/grczhbofe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gxeaannay.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gbttlhqvy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gzrtsbyjk.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gjodrtcwk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gwitkacnj.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gursqnwty.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/godskhbbq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gvtyewlcz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gdmopumjj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gbbitwphr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gypuriudp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gvofdobun.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gwlvfmmlp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/grtddodhx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gdnqafixd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/ggxuotisj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/guggjrrgl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gbjwcydtr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gxvbigppd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/ghdyrubws.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gimmpwcna.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gpwpxmjtn.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gbcdlfoel.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gebufroyh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gssffjjzo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gqupzefel.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gjghfazmi.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gpxpidhud.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gsgmitxzd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/grrjwpxel.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/guubpejlr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gauhmqbye.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gfktahkol.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gifewxohp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfahtskwk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gvqwkpygv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/giqzbsgud.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/glhpkdpyb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqykcdjmu.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gcgbtqsce.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gresmkhrn.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gikzadaru.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gtvjhwrho.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkuosioex.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gympeulat.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpmdbaycl.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ganwamnlb.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gnrflnvjq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gtllaxndm.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/glimrtnbh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gmniajpru.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gddsiipds.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gdiwzbggy.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gklzhvipp.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gtewhbfbv.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gzzustvoh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gmlnsvuks.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghrjgiqjh.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gvmexjafm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxemdcncu.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gjuympbit.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjafwlmgn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gnbxoxiqk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gbsfnmqix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gxualyvhj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqdavroij.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvoaoreab.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gdicfbzto.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glhkvynqb.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gkmwgubwm.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gahnngfki.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gyjlzrizm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/ghvdofnuf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gejtbqruw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gygyvcpel.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/geavknpbx.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gbwluqsbq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gsapcnkdl.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gvshorhek.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gcpfzvzkw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gtmzfmuvz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gzkyajspw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gszxrzkji.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/glsrnyeso.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gepfcoajn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/giclwsjfg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gtblrvznv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gzuwmgfuz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gyvdinmad.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdptddtmu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gndygwhol.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gfzngkkzx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gyqghqyei.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gjjdgqwom.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gojsilhdc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmaoinpwl.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gxoktzwyv.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gawbphntu.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/ggptnrhkh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/grgbmttit.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gpguzzeeo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gkzqukdpe.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gotolevao.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gtdvilowg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gcjaiehia.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gnyztvjnu.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/goihezpgq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/grsiudkjm.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/ganggtyyo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gcrrukknw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gsnewzgbg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gtajvenwe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gzowpvudf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/grxwshrsx.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/ghvhanpfb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gomnjrodg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gkhkjsidh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/ghogkyizr.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/ghsmqhyal.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzdpwdutn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/ghoaawwts.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/glmeawsdy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gjrzaauty.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/ggwkhmpkp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/giclmwksf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gubdpwzjs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gqnymldrk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gahiqlsiv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gxpycqdat.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gmtjeayov.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gexwoqrdd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gtzggqvpo.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gsnuhgzph.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/ghplscpqj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gllqrmpus.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gjbkwvkiq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gnbegqmhe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gesggdpka.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/ghjsygzgi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gmqxqlwey.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gmlnfriap.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gpqznyxdn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gtorhtfui.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gkhxvpnpy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gcqvdwynz.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gusxqzkiw.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gehrqcgqq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjhgvjntx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gxtpihxgo.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gawpyxuft.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gzzeifvnc.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gdttxzsss.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gxqdnzgau.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gilkvyoej.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/glcwrloln.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/getlhlgpr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gvhytjjlz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gvrcueafy.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gdwocnkhw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gzrydjzbu.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gfqdxjpiw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gczqszpuz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gbpeqylye.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjskggqnm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gyvwuqjxo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gyaxsphoi.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gxafyrcer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gkpkpzdza.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gmgvuavac.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gsyvvpnzm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/guiodsqwi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gzoqiucrx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwxieyfx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtptgxuxw.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gbxxfuxft.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gbukxpaux.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gwxerwbnw.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gwddzbyqy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gnwmqlaxb.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gcgjcvcsv.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gvstkvxgg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gjsifekuo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gvrhhqbji.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/ghsonpbhz.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gtufrwrqn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gkczsfpbv.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gnzdwrhpu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/grurcwclh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gwlnbgxhz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gufpdkuzg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gtuhjjftu.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gotwmgaak.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ghryvfsqp.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gezzngmic.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gfawlaopn.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/glopeplio.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqodxwr.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gcepaceqv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gencwsegi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gnumpcruk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gzqlewxsi.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gdznbwqld.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gcbbmbfxb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/goksldlij.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzecrpnqn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gpvaklwqj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghibcdpyw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gruvawqtq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gveceopnm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gfiqfrtcl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/goffvdqft.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkcbozf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gbkkovbqv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/ggwxvjdot.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtpynymks.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gzxchscax.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/ghlbwlani.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gmekcahvt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gxwiwltez.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gjjcqjrey.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gemvrrgdy.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gvrcegaoo.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gjvakdiks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gcukgrgcu.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gzikctyvc.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gwowduxgq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/goyhfwyfl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvummnwx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gffweksot.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gjimcdrki.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmzrgjyxf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gluzfnxec.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gngikullu.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gtvsurhxa.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/goygkjxmh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/glttrjpxt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/guzkmnjtq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gmrdaiugx.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gvhvfggpu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gsxyuecws.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gzlkacgct.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gdyrehbtp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gdvccuadd.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gcgzngioq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjcdfajjq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gfkblgztf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtssmdpvz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gsrtfmelg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/grxipsbku.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gfiyqfphn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gmqlahfkg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gdqaunycs.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gvzzpgqmt.sHtML


<!-- 参考信息 -->