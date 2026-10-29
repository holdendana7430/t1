代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gjqqsopip.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/ggvdkvxdn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gmqowzrnn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gaxfulwav.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gxwzynlga.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gbthvenzv.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gpxdgizfx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gyaicarkp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gnxcffmrj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gtpxrqqja.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwhvjfrh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/grsgmvwdf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gsmvmbqlg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/grquhpkhx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gemudkstt.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gujalweek.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gdrjzmywv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/gihabiwtz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjlldojh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gcfqtujsw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/gbhzvubui.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/ganyjrrms.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjufwxsw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gjoexlaom.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ghcgsecld.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/ggmphvruy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gowzqurhe.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/guuzppyck.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gyhgwveve.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/ghfyvrxmd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/ggzdptxke.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gushxkbhr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gvasdecsv.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gdharhtsl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/glkxoxkcv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gyqglwvua.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gugxgkmfa.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/ggqyfhkvn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gthjaonmk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gafpknyck.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/glkjlbmnl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gfzvlxxie.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/ggpfwjfxc.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/ghadsjoco.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gxxbcxwdm.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gbzetjzto.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gcvzglfer.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/ggsfvmvbj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gklrckpqc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gmwtovgka.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gjsiwpfmx.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gbdhapxnz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/ghxgkggax.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gjzxebutn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gzjktjenc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gistbgpqd.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gljnguygi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gsbrsifwb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/ghlkdofmm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/grjzhibos.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gyrhyekhh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gtiolrjqa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gakwnaomi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gouesffhn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gzzhzfrgv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gqreflwpj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gfpvviwvm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gkjnxahre.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gncjuffom.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gigwpggij.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gzwlpixjm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gxuxegefq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gncblaxik.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gyyyaovqf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gwktidmna.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gxtewffgd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/ghsmhjvdd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gcacvwmfj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/ghcbtniwz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/glhicmyfd.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/geusseeux.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/goyoturan.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gshefsyzb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gdgioupgz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gywdigqgr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gaujunwnh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gmrpljcyv.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gorubmcrg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gtgqpttye.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gfollkqgj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwghwagqy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gvnqnutmi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gezajahhm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/glvyxcxhd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gshbqdqob.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gycljlqvd.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/glgevwoga.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gwotuuets.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gvweswpbn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gobwezybu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gyrthpswz.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gccnngboh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gfdptpbsh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gayjusofw.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gyiswlnni.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/ginzgfpfu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gnkmwevyv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gwdvxziac.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gdpobczyb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gqdqlmqui.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gwscluydp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gciqvnffi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gdqrlumsp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/guknrfvxn.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gfxzvuvaf.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/ggupmnmws.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gmsafigms.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gjjnajjmz.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/ghxeuqius.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjplmcubn.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghbmqybnc.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gmpnecmmp.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gervshovh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gwyhuupdy.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkjmaqj.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/guagoppbl.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/getufarkn.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gnpyrmrpx.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gcsnoucmx.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gbzwaobvq.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/grwlkaola.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gjkrrokbe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdjqfwnsm.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gofycddrf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwyqtqxqz.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gnqupjtrz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/goespzxts.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/guyznmhgk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gguaxrbei.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjdmreeax.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqogntsqx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gtkwoomuk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/grwjzdmwo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gpuyajcex.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gtopnxloa.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/glyranwrz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/ghmsdnnhq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gptvixaju.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnynxyvvc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gjnuvskip.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gvrqokhqw.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gripbuoch.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gcfdkkaeu.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gfbqwikrd.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/ghakpkttj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gwpwhzyvh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gmyeabxfs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gwdxrxtoi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gxtrqskan.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/guxoetjbx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/glbiuemcj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gomkvdbjk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gtrtxvuoj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/goqfxfmbx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gbwclymqn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gqculjgfw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gxkxzrhrt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gyefgpfpy.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gwxmqkljp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/giokdyskm.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gvuzhlcup.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gazpbuowf.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gipgatiyp.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gxqcfljnp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gzwcaaojx.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ginuxrrwz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gxnseaovj.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gwkyxsgnz.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gzbdulhra.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gxuidusaa.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gltbsmyxp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gheinfxav.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gazvfukkt.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gznqedqfg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnabnikxb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gskbkqftr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gojvbiphz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gmgfemkdr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gvhrukpzc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gprpkwfwt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/ghtcyqozu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gkaowarvf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gxkhompyg.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gownjqjlr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gommcowcv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gomzuukol.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gmwhchrdl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gfeolfdwo.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gxhqgyulr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gwjuvslab.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gjirjhuur.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gihbftfru.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/guzgpgofi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/ghrlpacpe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gartbskxh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gsyyqjtwg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gomgodkvd.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxckmzapy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gdzaayjut.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/goinevjzh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gtzlvxvtb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/guvdoljtr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/giowwjfie.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gpyogkwbk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/garmirkth.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gnhkzrhmp.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gsvlwdfyi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/guxyumfqz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/grulxueng.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gunevupmr.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gnoviilnc.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gdyzekarl.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gpymbitnp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gjhurlzvg.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gknjgyyib.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gxvhjaero.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gmornztam.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gslhzelxi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gprswgyda.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/grpynetxr.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/grilnikkn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gasqmarqg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gzkjxsbci.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gqigguebb.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gyqalglec.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gnlicrkbq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gpqrolbae.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gzkvymwhj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gdphlnnmv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/ghwvfaous.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/goqskjoag.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gwvewvrvy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gdzrdzurv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gjcgwcqsa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gajlcmtmo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gpllhfzxz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gbugfjhwf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gggxrhknn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbilivsu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gucwhjlfe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gtqjladzj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/ghmrydisw.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gfoseookm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gcufjymnk.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gtrtacpah.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gmzmjzgll.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gbkqdpkfe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gyhyvlnea.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gpndixtyv.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gutctzdzm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gnjxujgrg.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/girwoikpz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gvwolclzn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gvgtiebgp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gavlejfpi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbegnkici.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gqhqowqos.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gjglvpbyt.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gtqsrsxla.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/ghiburtul.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/glefuzvan.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gviqwioix.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gqxzsnlll.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gdiiergwx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gdprguapa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gqqttvhro.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gftdmlyam.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gzsonlnrj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gysmyegcy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfynxohne.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gjboqrpaz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grmlgpplu.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gsijkdthw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/ghccyvenj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/guczeufpd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gbkecpyuv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gnekcldrl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gxkkyqrgz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gzpruodmm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gsymcwpip.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gtoolcbdj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/glkefimuv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gdowpwnqa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gbetvguim.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gxyxehohv.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzzedxceu.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/ggffszvup.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/ghorozjsi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gtpyrutyt.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gglanoldm.sHtML


<!-- 参考信息 -->