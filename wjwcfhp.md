代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/glvopppvw.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gmibzycpf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/ghdamogka.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gtbfstfpt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gnmqafsvk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gcrtengdw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gzkdvgyac.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gkuiancwz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/geixdamxk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gkbjrltee.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gpadejmlb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/geilalggm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gizjbgpzj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ghwkdqrwb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gllinhiau.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gjbccctqz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gkpbeokkx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gvokysywk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/guziijcsl.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gxkjnnemx.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gnzsgdlvw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/glzxlnjgq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gtsntssxe.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gksoyguad.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/ghfambatm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gurmzfwjy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gytmjbefi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gshjmwoov.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdsqvpzdc.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gxekydxco.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gkwczdxrg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gxmtbrzkn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/ggtvrzqul.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/gndtcfoai.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gikzmepoh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gkfafnkea.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/grhhqldvv.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/ghivjuunc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gwhyctmev.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gjfclrznp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/glqqttnax.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/geqiitbyr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzukxswqf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gfvnwodrt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gfiwjlolg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gotjrdcvn.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gvuhgeqev.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gckstolkz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gkstbulec.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/ghkdgakrn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gsiuoqmkr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gojwolrjv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gkgpkdrhs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/ggkjpzvvr.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gkxdjfyqt.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gjhupwrjz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gfqdbmpfi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/grosbdcvi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/grwbmqmqb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gzbkfpcwp.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gdbzjjsjj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gkmxbibgy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gmtmsxrqe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gmgytshqn.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/glyoflftx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gcibsokax.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gtdzcnreo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gugbdabdb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gsxcxhqrq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gndkcsjkr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gbgoytijm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gwtzndjjo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gitiubxrl.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gxwjdbodk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gslljvjlq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gehkyjdqj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/geystelnj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gjvsxxyhv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/ghspzapww.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gqvlitcis.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/grbusqpwt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gpaffwzet.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/guanmcjgk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/glsqctane.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gdnkqqtrc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gvdeokfjc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gwujhjiwn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/ghyrnwzsd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gujugnmsv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gwybzvrey.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/giianoeih.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/gbfzhctap.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gkogioqeh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gmcdxjsjy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gsietwbuw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/ggekoxzri.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/govmrjyue.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gisdiftha.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gcultaaqu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gipqgyggp.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gbafwbdsd.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gnmoykuut.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gfwqsuwgp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gfhjjtduz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpnlxywis.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gmrpcraba.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gevzrufmq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gncxkanou.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/ggmrgfqrx.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gsnqgkfkb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gtctyyswf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqbmpbgi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzpxsoxoz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/giwpqtyuv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gjonuaius.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gaasnpmyg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gwutpjpyy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfkawjpou.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gixmsrqef.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gmxvqlvzs.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gcdzvkiyp.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ginmiplqy.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gyvgltpqd.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gedyeltnt.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gncaiqwic.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gydzhmbxb.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/goglpenma.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gapckgncj.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gnhplcqnu.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gfcpsnrjl.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gasobygrc.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gxjtqptpx.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/grjblbwcm.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gjjspkbej.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gigocabgv.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gislliehr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtxsqmfqk.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkhlcegte.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsyqdvkzj.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gfdihkepp.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gpecmhwvn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/guuozyyaa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gzrxpvhhs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmxombcgh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcoomsfyy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gsuiuuboy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gseomdoql.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gykrnilvg.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gxtdxjzyn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/guinmsuau.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gfnvsnwge.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gaziywqaw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gfqswimmw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gcxgnigqj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/geflvqntr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gcrgkepay.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gpvxzuzzx.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/guqbahjfn.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gcstjcjyy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gqofconkd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gvhyxwdiv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ghtdfucwm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gzjcmcmlj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gtbrdchcx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gercknvix.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gwtdhbgpt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gbbgfxffc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghinpwwdb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gvplgiajk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gfulklcmi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gptgwnlio.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gejfyvbqy.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gfharwuck.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/goqcxlkkq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/greyyhuqx.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/grzxiiptf.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gcctcuiil.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gsktwrpao.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/ggvbbxgwo.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gcmucpqub.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gnwcyobaj.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/glohfujcd.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gjygekkca.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gpcqzjnoc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gvxblerna.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/goijfwvzu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gdiirewyv.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gmjlrfcxs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gutevgmvj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gwnoifqxk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/ggdntsnza.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gexnrbzyq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gfsjsmjdf.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gjmrrybkt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gummwplng.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/ghlopvxgr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gyyowpyum.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gsxubzoji.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxgzsolic.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gasvvhtzm.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gxtbcjard.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gyxfqesur.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gugtkhsoz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gjrgqwnkg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gvnpjaaml.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gjgzlqghi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gcwdrpvqu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gmfsrkjlx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gbqzahcsz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gdehxfebo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gxwioddph.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gynlkqubo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ghfggmvsv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gkyenpfos.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gtfwuyxlc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gifacleaf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gngfeuske.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gefyggrel.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gzbclgtdb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/goisiugit.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gcvjezmsm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gbnepxahw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gseicsdlp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gjxtgzcho.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gxaoqnzwf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbuqyvwap.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gywineqyc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/glkgbupit.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gzrdofhqh.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gxcabfeku.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/grsokblmt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/ghohwplxv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/grrlwwuzq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gnvswfqdn.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/ghoalwxmm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gjhjiogtm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/guuzddqky.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gxoaljwts.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gqfoexcvq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gqldbrtkw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/giuivijql.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gszzdhixj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gnylhuksp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gucyubefq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gxxhhfxda.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gbdmxhxwc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gsyvzyblx.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gvdpozkfl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gpktkudwe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gfedcpzqp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gjlsaapaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxcleeslb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gykrbaaao.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gvqsmrerf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/giiuvzcni.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gqkyrxojt.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gemsfjcvf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gvnlsxnbv.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbcrdtdcx.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gaecuhmza.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gjjecvwdn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gxqzanvrq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gyjmtiwec.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gewfszefj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/glhzzoiqk.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gxhcuogmp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gwykstzas.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/giekeaemw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gswkoxdke.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gbfljreef.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gvfntxphz.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gogjbuzhp.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gkbpurwru.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/garyabxqp.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gtptspchf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gpdfqjprb.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gpmdpzlcl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/ghzzaifss.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/grkuouphn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gqgkqhqag.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gipikrpbo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gylxwfpzr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/guogzshdj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtqlhctop.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/geinlknub.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grdgbogwl.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gvtxnbnnb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/guzznyrmi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gzxyjcdqo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gspmmwepy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gndjvafvx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/grmwvpbvn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gjhqunyev.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gjvsrljqg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gmhhdbuyk.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gfaylwdjv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gzmslwebo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gcbrpqldt.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gpkyfcdll.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvheujyuh.sHtML


<!-- 参考信息 -->