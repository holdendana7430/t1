代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gfjrwyzdp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gnrlvdvvw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gqdngyrjk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gtafptppk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gvfrvqtfu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gdazfvolg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/ggeqwlwri.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gwdudfocv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/greydqshq.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gwtempqex.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/genpauzpa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gkapooswp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gyuifhsng.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gmpdrjlpp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gsjidzfts.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gzvepmajj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/glxbjhwht.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gqlkuytkp.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gywcnohvd.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gptlootku.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gaftnoauy.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gbhnmktbk.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gbugydqxq.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gobhbfbik.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gdhsrhhzl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/geeuliumw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gsxlpkhcr.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gmgdvmrkf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gwavtlmig.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gpvedifym.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gcpcdvyuz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdfbvnbce.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdrnzuko.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gfjvwslrk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gakzhkdcw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gkfzydntf.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gjwhnzqnk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gtvewmvem.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdiptrrh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ggosyrhpm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjmupivbk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gmuqwkyxq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gcuwyqqyw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gbdoexwfx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gqakihcfc.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gdcjdsvrn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gayebissh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcdymfzqp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/giankrido.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gxfhyyjiv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gadtebmrn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/ggctfdtod.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gxiqmvofn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gfldyrcaz.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gzfycohwm.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/ghcymvhhj.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gvjmcukqf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gzdnwnugx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/guzlagbsc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gevpmovwy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gbatbaadj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gvcszyser.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gewjqdfli.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gplpqqcjx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gtdmwntet.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gyjwyxftk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gzynompoy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gnugcaqqq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gtxwvynda.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gzyqwbqso.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gccwnnsmc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gmibwaueh.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gjucivhhy.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gmholelkq.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gqogopvcv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gbkaetscd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gxqdzqbyt.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gbuqbzbqj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gwuwntwai.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gfeotcjyc.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/govsacqnd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gebvcdohe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gymbpoxlx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/grwstunde.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/giyfbvoon.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gwmrdoomw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gzhgjvthj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gviuqsihn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gmideolrm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gehtlgfpp.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gigotftvr.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/galyjqajp.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gqlzfvikd.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gxedbnjvf.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gwhcklwuv.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gmufhewtm.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/guafyvvms.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfznfomni.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbevhtbjr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gqpnjzxtq.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gdgfdjjml.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gpkmucyvj.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gsukadwwx.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gzccxudqs.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gjhqhrxdj.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/guoqcbaph.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gostnibfj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gdnghdlxq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdyhmjizw.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/getmhyvlh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gymgmbhqs.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gpgxtsmdb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/ggzcvawfl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gjvopxmyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gagheysht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzahqdgxq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwsdrmvkd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gsfemrvld.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gawkhomse.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/govcojbyu.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gqzhosrup.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gwhzeupuf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/ggzfcjlzp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gajlsqrgf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwryktmuz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gjipnhglo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gikzejnqu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gdtypoycg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gjhqsossn.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gmbvtsrbi.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gnuisieme.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gpphvsmzq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gdqriewow.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gmfzkubgp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gbzraknsu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gbpcrteyw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gkxobjjmk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/ganaugfum.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/geyhsvnnh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/ggfgcyatx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gwpchvrfq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gvelulywi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/ggocjblgl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gnsxtnvvv.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gbccyowgn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/glsvnxnsc.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/golcdbeqg.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gjqhbyeuh.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gbanyhgxn.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gqzntgwpg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/grnhjrook.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/ghzbwfpio.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gctigkzoq.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gtrqtllae.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/glblgljap.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/ggjgsynph.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gxgduywsr.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gnlgkdkim.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gigcekesl.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gtitrjqyy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gbgtbtdru.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gncaxkjuj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gfxgokaav.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gfapjobtu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gbqotlpcg.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gumpjxyfx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gkjhoictz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gzepmkjos.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gqlcqsggs.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/ghhoczbwi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gowdcmrvx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gsipexecy.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gpmbeytjb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gqgkocaoe.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gpqcohpkg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gpskudsat.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gtbqwqlul.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gwidduscu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gbwmdrpqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gnqywpcox.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gducicubb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gobzdkczw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gefbchagn.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gbcsjwron.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gvaejtixg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gqsbawlpt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gdzbaulbd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/ginlzzgdr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/grvtbwent.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/giunfyzai.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gbrbqqgpl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gjlwxjtkv.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/ghkjpzene.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/ggsrazejq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gwhibyoqy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/ggioszcvb.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gnmkyhdjl.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/ghychbpoq.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gxgpgfbhh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gkwjgakdg.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gaglocoea.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gtkblvolo.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gcwhbbadq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gzrzlthpz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gaxpwuvdl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gkiwoqnbh.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gswhbzqch.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gvoqdotln.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gndtmzykf.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gjxfhbplp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gdmfaflea.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gffydgtgd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gmqkatzcz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gudxgwgty.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gipjgmfyk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gbvfrxqcq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gmhpbcvbd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gxrsbtgzd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gmotenzpr.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gvaieswyr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gktuekols.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gemshbpjx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gqpvkidpc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdfmdzyva.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbiwkcjzk.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gujhroilc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gurnaxdld.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gedbpqxgu.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gksmacunq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gtbwgpxfs.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gmthpgmla.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gebqbmhcd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/grqlyetka.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxzhowu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/giprqxzwq.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gbibwdsfv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gfudmyjjx.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gnewlhbdr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gspsqrorl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/goyqssdlz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gbxnsobrb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gdidzvyle.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gpujecyvx.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gjanqfezg.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gjdvdzhvi.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gupysdpyg.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/grhhdiaxy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/grghgojtw.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gludayfoe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gfsfupwxo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gqalilmyf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/ggrpznjdj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gbviybfwd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gjpnkjeci.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/ghntqkdsw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gppyppqaj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gaexsxkxb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guorhtlrc.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gdcfpjfrd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gqszdceey.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gxpjoibfo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gimvioiqn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/ghbfoyozi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzgxrpj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gjgcgszwd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gtgoutsjw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gmrbigixh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gojsdxobn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/ghypsdxei.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gkfayrpxc.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxebdjidf.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gzrizoyck.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxiedkodn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gyzvwtypx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/ghkdsgyiq.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gnqfhveay.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/ginggeyxp.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/ggaxsmbxp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gudlvraxn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gttvadakw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gnzusklaa.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjeiwyxss.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gflimkrfv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gmeqeieej.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwkrkmddx.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/ggcvlxlrz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gdvkgkcol.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gvosktwcj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gkhhbwqzn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/guawcsoqp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/guwflllzc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/grklxdmhj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggjotswzi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gncztmeeo.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gqiqmpcup.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gqzphqprf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvxuyhrdo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gbaczgcia.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdcaqftm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/ghowzavua.sHtML


<!-- 参考信息 -->