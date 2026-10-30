代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwibznefl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpbqcxzw.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/ggnqbijmq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gmbajjggj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbgxbvy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giisbmklz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grezsjsbt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvpfqyls.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gciggrcec.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fanxiaobao.xyz/Article/details/gxggboece.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gttlbfprt.sHtML

[B04] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghyvqjeta.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gxrhlppcl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjkyazqe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvrqsrtg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbdgfwkqg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/glodeuvrs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwztkotep.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcpycgey.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gssclrqki.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gzjuxwevo.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fanxiaobao.xyz/Article/details/gwomcnadr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fanxiaobao.xyz/Article/details/gecxcxwgw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfouhdulj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/grsanazpq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvssarqiz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywsultzf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsulxjdzu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/guomwqzvk.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/goblgzaep.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fanxiaobao.xyz/Article/details/gidyvlxod.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guurpkaex.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpcwfopde.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnrdfcxuw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/galjrnqfp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbhgqvmg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/glkifazts.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiguttzi.sHtML

[B07] while 循环
来源：http://baike.fanxiaobao.xyz/Article/details/ghuaoufgo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gjnaighmf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/grfkziyoz.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gymmitelj.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/glwbabndn.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gftojsrxq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhojelys.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fanxiaobao.xyz/Article/details/ggxnpaqyr.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grgasqzcn.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqttksls.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/gvikugawd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdqyloyo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhyiwbiz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gdeuvaszj.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gooiixeet.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gltqtexbf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnmmmsfb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gphhdxjkf.sHtML

[B09] break 与 continue
来源：http://3g.fanxiaobao.xyz/Article/details/gtiqvfzip.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fanxiaobao.xyz/Article/details/gwbmkdoer.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkswzldtj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/grihxbobm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaymnawfa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfqjmqhnr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlkkoqyn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/gutysxlbi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtskzweyj.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fanxiaobao.xyz/Article/details/gbmtrhgst.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlflbwvk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsixerrdx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqxyhdoo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gveabyyqg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcddkxin.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqpoojxd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gatxomumh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukxehlom.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/gpvxrwbqk.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gotwmdsur.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gausnnlrk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqxjhlqy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/glllpomoc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqsfmpfz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gigzdbqag.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gzktgiuix.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrfysjsm.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/growceves.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fanxiaobao.xyz/Article/details/gknslwtjy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzygomruf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzipblwfn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/geujilcsg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gnotjjays.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjowhtgkd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/gfexwoxtg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfjccfhn.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncfogemd.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gdwsfyxvc.sHtML

PHP:  is_numeric($x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghsdrtkpp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaekgotky.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwbebzqgy.sHtML

Java: x instanceof Number
来源：http://3g.fanxiaobao.xyz/Article/details/gitmhpdkg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fanxiaobao.xyz/Article/details/gwvaljvhw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdlcbyox.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhlyyjp.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fanxiaobao.xyz/Article/details/gliachuaa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwsbattu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gigvqnwxb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gndzvftih.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gibqtjjai.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusvgoanj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggowzroyi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsozorejq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdsvsygz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbzliprm.sHtML

Py:   a and b or not c
来源：http://wap.fanxiaobao.xyz/Article/details/gzrvzdjug.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfbqgxyh.sHtML

JS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gfpuhdnxf.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gypzwlmwk.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gdnmfjejj.sHtML

Go:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gkijazkow.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/goscxcgpe.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxqdrqln.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gkalwunrh.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcjhqxyc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadsbteoh.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsljssnx.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfrwadoh.sHtML

Java: if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusjqrrtg.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gfpmokmao.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzldhkgv.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/guisqadxd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gviliplqf.sHtML

C. 函数与作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gmrwopkiu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcqckgbpc.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvhnqdfy.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gdlpcaiwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gailobois.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzlwdeped.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gybjdcmyt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdovubml.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/ghdplhxot.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gfesnsodn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwbqvat.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpglvhkyb.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuchawtv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goejyzawq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcllapab.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/glsbcxyiq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gvvammdke.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gscrgrpog.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuldthpu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhvruqea.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibpazrwu.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/gwcvgwvsm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfwkujlw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbmknlem.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldhucfiv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gndjtcbfn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggptmdxis.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/ghotnufzy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gzawwzshm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fanxiaobao.xyz/Article/details/glikmrnrt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fanxiaobao.xyz/Article/details/gymwdaloa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyiqavza.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtouejgp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdazmnyl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxkdsxxc.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/girdhyaoy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuuprkdv.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaioqsoyk.sHtML

[C05] 返回多个值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhzlfbrj.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcyowjgc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqblttpn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxebkczx.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejhqexrm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbjtsgct.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gwsehaiod.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gpzpoudli.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/gbbyfckns.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhozikff.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrxejkwp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fanxiaobao.xyz/Article/details/gwcyrfiiq.sHtML

JS:   const square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gywethiwy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/genkeygyi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/goqlxguns.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcorfjpvk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdezacxpc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxwmpbmh.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gyjlrsamv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fanxiaobao.xyz/Article/details/gghebamlw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gwekhhwho.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gyrdiqdec.sHtML

TS:   arr.map(String)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvadkqkv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/glkzxtnoi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdnhrllh.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fanxiaobao.xyz/Article/details/gocmyalsu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpkfiexz.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gomstgwfn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthylcgdv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzfdwqes.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkttcrjch.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmyelfxa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gayqplizm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fanxiaobao.xyz/Article/details/gloepzwgy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/gddhwuval.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszzhdmrs.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmwyvqow.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxioyfiwa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gueabwisw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gwtvnxssm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gjlcgoboq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gasmhbspq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfhpqksb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdujdmko.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gymwneqzh.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gvfldlgvf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gdblkjsis.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjlozjav.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gywojxtwa.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhupdks.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwppzwym.sHtML

Go:   花括号块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gnmenoiuj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gdcwqfndh.sHtML

C#:   块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxfslrjt.sHtML

[C11] 模块导入与导出
来源：http://3g.fanxiaobao.xyz/Article/details/govisxmgg.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsflcfffx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/gyltyarpe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gebmbxkxu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/gkdbcfdye.sHtML

Java: import java.util.List;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkvhobig.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumzqjaiv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gcpchyefv.sHtML

C#:   using System.Text;
来源：http://baike.fanxiaobao.xyz/Article/details/givbtekzn.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/ghagkciof.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaisvooh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/gemcwzzxu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/golypkaum.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdtxscnd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fanxiaobao.xyz/Article/details/goamdmwvh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gavurlvbq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaepsffoj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxcgsiko.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcpkevcr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnvxdpmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggxnizibm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhffavwr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkobupvzo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuimmsnn.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhroiac.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fanxiaobao.xyz/Article/details/gtneoirek.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fanxiaobao.xyz/Article/details/gbrzwwuvw.sHtML

[C14] 泛型函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwtduhal.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fanxiaobao.xyz/Article/details/gznyawzmj.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gbeqejaoz.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/ghccdsfyy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gapdkqway.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghryhjmaq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/gcubixyyw.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuqirdmm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/gptsvethg.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzogphksi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/gkacmglwh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gjveroiva.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpoxbdkbp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggthxaozx.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gwakkrrgd.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gttjvrmfd.sHtML

Ruby: a, b = pair
来源：http://mobile.fanxiaobao.xyz/Article/details/gkainrojp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/grutzdnwh.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpgmegix.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fanxiaobao.xyz/Article/details/guchhamqq.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gvttwlrkb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsavbltnz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/gqyzkmspb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvxjbuerp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fanxiaobao.xyz/Article/details/gwxbhrkdk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhbicthd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhhmzdlv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjybajqv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/geixypcxd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbrkdaoyc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/grefzbpsc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gbbfockhc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gatmzdtdc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowexirhs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fanxiaobao.xyz/Article/details/gzalpjjci.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/gngnguevk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gtaovzbah.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gstbajall.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtshkdae.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gxudccqbi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fanxiaobao.xyz/Article/details/gmdqspqwv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvjmnvyp.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gejsmsxsb.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gekgslhmw.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gesxwcckw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpambzdte.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fanxiaobao.xyz/Article/details/glfknrene.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyclagrkx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdvjyrlp.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gleoncauc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnvllevp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gdtcwekbo.sHtML


<!-- 参考信息 -->