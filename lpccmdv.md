代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gtoexnbtg.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/guhzaicxa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gzfqurmev.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gymapoykp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqaurwur.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gxqlzgqls.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjumdlxaf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gyridizsz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gelzrnwty.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gtozbzcjb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/ggejygidr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/gfvkisima.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gjkunlwws.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/grjwovqpo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gojrfpffm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gatrpatva.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gwwkkrcdi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gxtviarzt.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gjfjiqcja.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gzbyctrpd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gugkezjyi.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gufauaseo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gfmqynsll.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gmubtsxsl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gvcnbieob.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/giydceypf.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gynfsonfw.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gfjozlmqf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gjjyktczr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkvxfsps.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gcujkipap.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gxlzujocv.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/goizvqvsl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gdhehpxhf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gbkusycvm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gearrsupa.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gvgovczmd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gkaadeexj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ghgyxqvjs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gkkfqdtbd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gtofrvtxf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/glpougjow.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gncoadnsx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gvdcoysti.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gkydpfsrs.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gaklppliu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gljuvssoa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/giomefqcu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gkgekwdrc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/ggqnqkzyv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/geaimvsci.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/guafajjnz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gmskyrrxw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gqnfttybf.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gcigsuknc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gcxbtbrgu.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/ghwufropg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gtmkkweup.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gujvtelpg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gdaicncyh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gztxkqyvh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/glmzjgifl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goycliwnr.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gioxibupu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/ghuqsrdxy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gnuykzvqo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/giervvpyd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gryuuktgl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gxwejnimb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gwkokbwgy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gdtvgezfo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gimtesfhv.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gnxsvcjdj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gnivbsxhf.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gdurcllmo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gxugprkve.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/geafspqan.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gbgoxrlwt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gmmgtcssz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gnaahvqgn.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gkznonbav.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gialuawkd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gyoojszaw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gytxmxqay.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gppkthied.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbkdjohlw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/grpcnuted.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gyljsgtek.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gzeylzkpe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gdqwddsia.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gnmlakqvs.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gogilsqtx.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gatyyjwbr.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gplvwpksb.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gtkqunxym.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gscuesgdw.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gbvgowicg.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gzblozpvw.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpgqnqylm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gqowjozex.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gzntoivhx.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gdibztiuz.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gaxbupcpb.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gwsitpbwx.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gsijrfbyy.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/goemujfts.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/guopfbacw.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/glqfvkasg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfbajejvr.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gviknwiku.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/galfnitec.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gyqhmgxvi.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gjpewfudv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqubfjwcx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtartpisg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ghgzmnmzo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdoirhimg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/glwwwmejn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gsnggklzg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gzucvhvcq.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/glefxryqe.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/goeyfafgb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gdxyyfunt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfxjgipzv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/grcbxglar.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gxhdgeayf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gmtteynki.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gxdgqpsno.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gxjumjnsy.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/grzrgdrpi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gvwlgppgn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gqvbfuelu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gtuaninjh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gqnldgqfo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gemddodoj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gysaxqhro.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gmbsfoskx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gtjvcqqie.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghgconeed.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gxdrepjeo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gpfmppejd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gxntgjwze.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gphncbgin.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gzvhhwkdo.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gzcdgdzrw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzivmbfgg.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gwydqvpoe.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/ghlqpbieg.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gblrxrhjk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gtplueniv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gpksfizgl.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gabhicjnj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gyncwrdxm.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gdblelvad.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/grncyfmva.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gbmszoacp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/ghcevujhx.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gxngfgllk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gbtqabezv.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gsicneyis.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/geplgtfnb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gooondypm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gmdsktlhf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gumpllbkm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gqmnapslm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gwovaymev.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gnvpjevnv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gsjmlqred.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gcuwwrujz.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gdtqqybrj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gnrabgpin.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gkeujrbnp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gixcvnqle.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gbuqxcsoa.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gcaxkvfol.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/grieyojeb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/grcutdsjm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gmlnotrql.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gincrlvet.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gevxmsjxw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gxlnphmjh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gboyshkep.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gvvjwbfae.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gvzrusoku.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmsycovqs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gqbkrnujv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gljucuawi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gmnafstzi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gxczctpva.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gjkoxbwxm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gvrgjwqcs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gapauymeh.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gblviblfp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/ginbrhzew.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/grbllmahq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gexrrspgq.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gldwsniwv.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gztlfdyai.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gtckcajcp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gvbxgdzcz.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gafbffark.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gfobznvbh.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gzemfztew.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gjbmuevti.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxuxzif.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gqparjrvg.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gosglumxf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/giddwfwiv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/grbokdwqe.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gceeynuow.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gckktstiz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gikxpilzx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gsosxdvth.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gbrqtuvcz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gkdyubuje.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gfdycdutd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gzvemniny.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gsldmionk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gfvxpjozb.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gwniobknr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gvvjhlqfx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gkirdzobg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gwymhngsk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdwfvehll.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/glbpncgwq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gpxiyxxty.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gskjztity.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/ghfcbehsh.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gyfxhgigd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gpxjhdqbo.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/grvupannp.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gyabmlpao.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/giyvfnnjl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/ghipsqvut.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gwbvyepdm.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gpvxfxgrc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/ghfbcccpo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gdqvpkocx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gkgmuzzxf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gblxktmxb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gncuwrtnk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gtlybdabq.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/guztqzaul.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gfblhncjh.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gbvsgummg.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gcxrjbylg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gylqwylpq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gjdsvdzem.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/godbrfuis.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gjsdmuevx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gxloogczu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gawqwwilz.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/goilbznvw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/glexclwox.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjwqrdsdz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gypmhcyoy.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/geomqegqy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqwvzdlby.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gunitfvim.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gxxcbcbtz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gdnugvgps.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gaevzavau.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gwgofyzbt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/ggsmlkqjl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gjdjmqtxa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gzoehemim.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gnxawwskh.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/goeixgbpq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gfjiffcxq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gheqzndac.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gdrgejzud.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gjdpmacwv.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/guwlmdmwn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/ggccewyui.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gwnmiltfg.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/glrycinhw.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gnskgwofe.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/grpkdthca.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/grtunmwny.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gkrsexhuo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdjszdgmf.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gijkbsipg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gsdukuivt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gedsvfxgz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvstvrude.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gvkqujrti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gqgkecmdy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gqfdyomrd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gafeugwdx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gyvuosyus.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/guaunupim.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gbhxlgyfz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gzcarehpu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gzegkhlxb.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gzmnpywvf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gnkytmhya.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gfzwupqnf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ggsnpzmsp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gvkxbsntc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/glebqcael.sHtML


<!-- 参考信息 -->