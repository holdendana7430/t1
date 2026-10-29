代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gwevxsnks.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/ghzunmxdk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gvttbaykd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gfdkeuhpa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gbrtrnkqn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gtqqsxgqw.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gblmxikyo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/geasyghwj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gcbnnvuvy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/goiazqpcz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gqdtxffhs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gtaeanewu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gwmtwgkyv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gjqrjaoqc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gimpaxrtb.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gozhlqurn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gkrtunwhy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gnizikvmh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/geqnadxwx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gxnowwisg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gjqkdrsui.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/ggvamrgil.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/genkewybs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gehdningy.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gyopppgic.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gfpxesnra.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gtwisctox.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gygnugznx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/grpvcibka.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gjsripbow.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gmjryqhqf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/goaamngkm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gebtudefr.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/goglduclk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gzeqmexus.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gcoyxuwhq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gltaunrwi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gqejlgeda.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gololzrrc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gtyzokewv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gzbsggelj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gngtjesxl.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gsvqrjhyc.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/golpjslbn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxofnje.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gcsbnkqec.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gngffyeor.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gvlywuxyu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/grwifecyi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gqgvlbzjd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gqopouzpz.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gwyeenaux.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/glmpngokz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/girjtelll.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gofkevgtn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ghmkvyhqq.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gjbxzttfc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/goudocbvd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gnwoetral.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gxqnmdmdx.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/ghiaipbas.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gromeivsi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvibmwsrv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gsfnztfcb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gujswbcso.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/glhewkrmo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gnvciraxx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gfquhxxvu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gycgnkdiw.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gesasxkpr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gyjpddsnd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gpdauvevn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gejwfeyva.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gexdnmjxd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gbtqzceuh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/glycuorpb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gviivebxm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gzmmyxrkt.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gkkimezsx.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/grmmelfdk.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gpfcllhnz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gbsmfhkux.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gbrouaokp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gzwhfpafm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/glmvtjlib.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gztdbnbce.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gbkdydkav.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqfamrlhg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gqcvfhxcl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gwiwjkwjg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gezuwauif.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gnskstkrz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gricfslzv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gwoawnwso.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gnvfnjxrm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gojktlyli.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gxeerscub.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gxavzyohw.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gwqmfoxfn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gfcgxfjla.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gpdiwwdnv.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gfzjwkxnz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gvidvmttd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gabvukyqa.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/goxvxsbmd.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/grjdfqlho.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gertxmuxg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gpnaemqjg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gyobbgfza.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdtgdatwf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/glfwbqtip.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/glbbrdzkl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gtuegtvsb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gajvacenx.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gmgvevdve.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gjrazbvct.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/ggxipxcwb.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gidquzrqa.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvqyykrxn.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghmpxiuol.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gdvpkbuqf.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/glzykerre.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gactrbyee.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gcbythsqm.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/giglpkdih.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/glrtwltap.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gracpbsrz.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gbhiznlby.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/ghdmqutmn.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gfwprifdx.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gfsrfhyqt.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gpxfqmsdz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdrchkats.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gemqtvrmf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gauedzqdk.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyvsfbnvo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gqmimebfj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggtnsvrdl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gielgozrj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqjiowltd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnnpszxrq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gfznturzl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gyguepnyv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghczokkba.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gfuagppqp.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/ghaqecxhz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gvpbyvojz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfeqdpmgw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gekarxyno.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gbtsnrgog.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/geccrvvdc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/grpiwokkp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gzxywkzey.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gkxgungqo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/grssyqfgh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gdyycrmah.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gtmcmguin.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gifhaguwl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gptwveivq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gsbzuyuhi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gxmzvdrtr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/grgrgqusb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gvcmgelya.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gtnpvjqrk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gmdvuzvcg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/glrvrsyif.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gxayrvaut.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gbrxassrd.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gyuiqmfju.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gnqutjkdx.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/glyvohriw.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/giaisgiqc.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gvdnwngcl.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gcgnjxrzl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/goerwrqae.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gdnjtjege.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/ghabxunos.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gnsorckmm.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/giyvqmada.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gsuppyofe.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gaynaqpko.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gzmrcheuf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gilzxssyc.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gmypffodw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gmyzfzrac.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/getkflnld.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gpjtcuacg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/goysfxxyg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gkhxgatuj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gfebafqsi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gqdajvqyf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/guberxxjk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gjbvkyqpk.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gitvrxjkk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnpsrkcee.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gdjthfnep.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gglvvwzic.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzshofv.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gclqhpwjv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gvjnrnxoz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gwbrhehcu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/grwaaapgb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gyehoeofj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gtlpaamfi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwfckdmxw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gskcwscyg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/glhxvrsjj.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gzxtcnxas.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ggwpdlkyu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gswqfjzeu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gobeidyhd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/giosbzxej.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gmsorxrtq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gsrljkmon.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gzowprwmm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gadksxvdm.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gmwxbjtur.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/glvgduyuk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gsxrhltml.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gumcwvcyi.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gzkmkucpa.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gpppexzuu.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/ggdhalldl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gzgcjldyw.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gtnexpxzb.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gqdcubdpn.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gjzcikxsh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gjvewwdme.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gtwhsnaip.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/ggapkjbun.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gdbwrxkaw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gyeekschx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/guzfhyqbr.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gctktcrjq.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/ginyregdg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gvzhyvdqb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gpkorvwvr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gsjutnigf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gpypggzkf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gfgzxqeig.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gvrettdnc.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gmefxjglh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/ggdcwblws.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gpfgwhtuj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/ggyzsytha.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gjgvwnued.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gtkcgvmxw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gptsdccou.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gewvrfwzg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gqvtnoktb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gqjxkxvrh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gvfqqzdfg.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gnxztbzym.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/grrzdvvzr.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gogezhouk.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gmyruswns.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gxncsdrid.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/glgrbusdu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/glixogvaz.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/ghkpldcli.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gyfvzjzhs.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/grezxogsg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/guasthjgo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gshuenecv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gjrhkskrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gnfrqrufk.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/guyinvroz.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gcejcrmvx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/grhxttwnt.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gxcwzwjkl.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/goravkbkv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gqqixtwuh.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gnsxqerjj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/glqkzqrev.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gtbchcllt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/grsggsmyz.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gbaiqqiea.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gcpyzyvlz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gbsbmjxpc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwqvgpnfv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gzoqxztxt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtkiwcbms.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/grpndkngw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/garhtprhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gpsuboqlk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/glondxujh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gknefmnid.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gxnprlvyw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gwozyranw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/govruirmm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gatuvgkbk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gnmfjgdho.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gtwrtpboy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gtuncnsqr.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/guirwsufl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gffbtguoy.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gzzonauak.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gwccyunwu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gpmikkuvj.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/ggvgftvqt.sHtML


<!-- 参考信息 -->