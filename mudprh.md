代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qkufalot.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ecieilyu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ztlncoee.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2yezgvnyo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fryoqznd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttduhdie.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bknzjucy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nmrmzflx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lskxfplw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2svjermua.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ichkdtic.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wqxelpsu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uffwfjih.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2wgnsfyvg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hzlpqrun.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rsgrzpwe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mxdaddzi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hyjslirv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xcqvtaqv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlqselde.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wuyjhyxl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdetnrb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2syderdlr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mvpprlzr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bintnapw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2apotcnsq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2chrmbhzn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vzvhwyqi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2strkddzp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qiednwkw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ovqprtuc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeiupaxq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bmurezcq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwkmyoua.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rpfutckw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2oaacakri.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fwzpvqvg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2cphjxdhi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2uqpveukc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fcozgjhw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wdvbisxq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzjldwim.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlqcusg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qnxpqlnw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2unmhcyuj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dxpwccdc.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2enqcgymm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kvrqcipm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pofbntzt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gclyfoib.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fxhuppvi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xvknrwnq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zfelldhz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gndopukm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2saqizodh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cjfrjidj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2imrvqouc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fhjuheyu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tchsqbco.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hpcadudk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyiaitxy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjwpbuva.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ilylsvwz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2erbwvpmu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tuesizaq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vwlajmsh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ywiwdyvn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2txxrantx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pdxwiabx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iltnakap.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2vmkezjen.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fdnvkerw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bgmcqcfy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwieprso.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2apbvqdwp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zbodqhpg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hycuddvz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cwtccyde.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gylsrscp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qxsbtihe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2fbzwiogc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2judmhqdt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ardqxtsd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbhjsfnp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hvzolvgr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2aobtquhw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ykrytznl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qkyfdkyr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wpkgodcb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fktdiwwi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2krttwqcf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2oetgumjg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qmcunfzu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wwferfnr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rfuxwsqu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajygogau.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrzrtsav.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2uawjnpxa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nkesrdbb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ckwayocu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ewywtzzj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ofkdehaq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ncenmouh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tybygdoi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftqmdlzn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqksanqp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2grhusaaa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhafhih.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eidpqpjs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldvufxcm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vamgaifq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fyqgakks.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vzvstbsq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2chdfbilp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ysajvjzy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pzqddjhk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2umpyztxj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zvoncnxx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kljngduk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ixqzffrd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rvizpega.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgssuppv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lgyyshkk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2abfgguyj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tizwmmrn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2odsixwmc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2okaplltt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2scvnkmkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgnhzpma.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vbqoscgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwpwrcuo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lqdcmjwm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hhhpmpdv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfcbrapi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lajrenwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2btnxlhti.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmujwoou.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rpcynqfl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2glzkpbpt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fxegcjmg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sqmynqzp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ubtzzmxx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fabvnkar.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrmlobuo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qcfxniss.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gymkhnrf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdjxmufi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2twdkuufu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2iikbslyh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2yeeuemfo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hrignwst.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipavmorv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2azuehkam.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kfjcseet.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvwhpghz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2eqaelqck.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qskeowmf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qrfdfjmw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hwpybhog.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mvkenlwl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hbfdmxkg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fifvdqhu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ahjmkgnz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2alpvcswd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2orylivbj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nsthrrhl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugllrgem.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2yfibonet.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eyrvyoth.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tfrpaxjs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yargrqcc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lbyulqbu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ovpkrwbs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nnueaxuk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ocftoulo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fqvxdqge.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xjmxuwri.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2naafjwhe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ifgzxkhh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qeglybho.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qmrhsdkr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mliidrud.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bdhvknwd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2keudrpae.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2euvqgjhc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jlcysvbo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2txrvrvow.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bmkhjnqz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wsvoyjrl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uhrtkzbd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bjtzmfya.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2uwwovknv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2danqmdub.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rwpqkhgq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2omqlaomo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2puzdvily.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ptqhamtz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2owusflkk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovssrhzl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2enzpwzei.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2llsbxkyg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bdksncua.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mudmddbn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qmkwiqub.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxlzsvno.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2loewtrod.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rkyfyccq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2acajkcbb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2caycevxr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2etnschne.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yhvjaqgo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2oeaxpznl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqcixkls.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wzqcimdy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2njctfagf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nwyhrvfb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sohbsmmn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ocpyhash.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jfdjqfht.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2sxkzxklc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wppmrhag.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qtuqfcpc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gxqokgjj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2caaajdkt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wfmagvaw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2uiqvfjjw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2llxlbgep.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xitlfnsi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2mvuyrcmt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ykanfpyn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ebgdikct.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2htmzlpsq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lprfdrgh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yqrbppoe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2orgblvcv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jglutcwl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2npbausis.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pofgtjdj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkpeyrpr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fthcxdea.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bqbvisvx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nglricmr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yksmwzkh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lalgujch.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2guseflwv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tqjngwub.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cfzddalo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ruchxxvj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hkokmrbv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ckzptrqv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zqpuophe.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iyhivncr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fxyruedx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tkfxwkyq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gsbqoazv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ytpfunfd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zocpfejv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uzzhlkvq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2obvclxxq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2extvtxgb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2baogeuni.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vhmkmejm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vsmlwnta.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mwffqpoc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wamvxzts.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kzrltdiq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ndnfwvht.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tknhdxuu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mhainefj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tmtwdccd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qqtwwngn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gmcruunx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wyxkvvvi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzodabns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gjfhwcxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpeqqgxv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2oxqffjet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivrkulua.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2deogpfqe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aygcqlhc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ygppdctz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wormvyiz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hynaceps.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zvrpjbhn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2yognmmyg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sxrvyrse.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2apwturhh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lsrplmcf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ccujwhql.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rsupugjm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eescjfot.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tgnwaedo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jloatxmz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ldixgyna.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nzuimddg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mivuvrms.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jrwvzifx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kexdnqda.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xzeeirkv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zkpnefww.html


<!-- 参考信息 -->