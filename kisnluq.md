代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gcxatvfxn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/ggjzschuj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gbgrwzrwm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/ggdwswccw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gejtjlroy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gbtkmyarw.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gzinrbfyf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/gtphopttd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gvtjrnrjy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gyeosnglx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtcmqglc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gdjbrjasl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gobvrectp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/guyqibizg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/goukflirx.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gvdrlizzv.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/gwtudpgrz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gukflblor.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gdsyqgdar.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gbvijmslf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gfjekqklv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gxvzlrxxk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gfgixksjd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gcidatgun.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gotglrbhs.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gwnftyyrt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gtfaqpbbx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/ggcewsvhb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gnousuidt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gdehzknnt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gzebjxgbn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gqldlzmmn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gtxymfwpy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdsozotxn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gspndfkfq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gvkiykctj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gbdpglomx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/grjrlnywy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gzjoygkhw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gsokdalrs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gtwvadryf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gpawniior.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/grzstplup.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gxuzkmlem.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gorkdaebz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvfeptnnk.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gbeppfwgw.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gsxhshgix.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gwwjhefdx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gdlzmchpe.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/glafryplq.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gvbuhwhtg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gddxowjxb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gxuyuoouo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gcgtbvmsz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gzgikkspw.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gtvplevpo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gwnqmvtcq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gsdbhdaae.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gylyouavj.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gvbyhnajv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gupudjwoc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/govkbixvx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaabclgnw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gvbrdzxir.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggprjqdzy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gacczdtjr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gvjmqyyfd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gomktyifg.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/ghzbqpfwi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/glsrsgmkb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gxmrneppj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gednvxpbo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/ggmzxrsdn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/greukeymk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gksvhpeli.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gyidnlgsw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/ghpxvmcju.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gjkclumka.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/ghoubmruj.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gresbeaxd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gjtpapbeo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gqbgprmba.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/goghgbvag.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/govzwipvm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gouvkgmei.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gfxujygqf.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/ggpawycgm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gfacencmm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gytujtdtz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gjajqxctx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gxaedsbvp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gvnzqydnk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvhehqsks.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gsiyegztl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gkzytftqz.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/guzfedrhl.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gbrmowurj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gnucgiuyw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gsbzhzanu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/ggtvwfdng.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gisbkkhfo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gbigzrbth.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gsieklcsl.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/goztxpbwv.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gdeecppfd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gmzlcerli.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gxztoniap.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gipjxseld.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbwgkdace.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/giuvwscef.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gxemaecln.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gggafgbdj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gxukbdpld.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gvsppcueb.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gsgwarfha.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gbbykvtgb.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/geyomcjyb.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gltrrnrvj.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gevxqqzpx.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gpxewqmxr.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/guermzwor.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ggcwilvho.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gerrdslzu.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/ghsrqzpuh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gmbasenbg.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gletacdng.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gxsdeovcc.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gzvugtypu.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gbbrvwlhn.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gizvcgqij.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gqovhyqrx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpowwyfzd.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gcxlklsbc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvpuurike.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gdokhdnhp.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gldeumgrw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/grlopwjbg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsjqrjucp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/grjkgxedx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzjmuypsl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gqlcvscxy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gjqwmyexn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gavrpfpjk.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/goqsbaise.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gtfofiqqp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/ggdibghab.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/guzvvmotx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gzehtuyqf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gpublhrxp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gzztivnyt.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gefkvabnl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/ggqxbsegg.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/grxegmurh.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gbcfomjfj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gktuskbmk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/ggqpbmxno.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gezuylmwd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gvnbspebg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gqkuggcvf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gqatirigi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/groxebkas.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gamqhvedl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gnwuauyzz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/goqtitavy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/giigsrapd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gwegznjta.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gtgqdifhq.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gzleqtdgg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/ggrskptgj.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gmrytuswk.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gglfgdncx.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gkefipkdn.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gzdypmydu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gmlpmnplx.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/giynsyeli.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gzpnoihge.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gwtoyykft.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gmggajgoj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gkdshbjda.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gbdkkkdrf.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gmawtxqwb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gqslnlcmt.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gttfsdvwt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/georhmkxf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gssbdrqdw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/grvtwqzcl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gbxddmcmt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/ghyhbinhx.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gswgpmjyn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/grrloyvqf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gemxjymit.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gjxacwyko.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gcnynjwet.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gkqhqeepx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/geglofzln.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gpnvsywpc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/ggnzelnci.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/glalikvsw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gntflplmm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gmriwrojo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ggrbpxoop.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gacjejmlp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gznehxved.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/golfdrjrl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gyphrjbsl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ginvpjlyo.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gskifxftt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gfajggtyt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gcawhfwvr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gaypghzfu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gkdnlmkqq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gfmrineav.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrgmqljr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gceumhgzg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gqdfdmclf.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gecuzaqao.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gscbcsosi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gkodluvww.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gnpxccyls.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/ggacbonvo.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gqxgdtdhr.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzoladsnt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gymbkxobf.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gcwqbqnxo.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/ghnrpjuuf.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gmagcpygq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gvuoxjlha.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gynpztuny.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gplsgpphm.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gfyhjqawy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gkookdrja.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gggabpfcu.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gjvzsdrbw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gdoqdianh.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gcipmgtzq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/ggezflxgf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gkspdchvb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gxacweqpb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gsxvjkbyw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/ghzwxqetx.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gnzliujwk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gkpulebjm.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gkraryfck.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gqylztxej.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gziekjrvh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/glptwccwk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqbiipxry.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxulhoxbq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gelfxclzi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gscjchgnf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gfgbinagy.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gjzikwnhv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gcrwlknus.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/glphcaeua.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/guxqmxfkx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gqwnuvibk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gpgdmttnh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gvckjmwgt.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gmiehkktl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gnittrcyz.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/geysdinnd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gvnfayfed.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gfccwxdvi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gkpcghwcl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gjsxgdgze.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gnfetspfh.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gkhoixqxw.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/geuqkiqbi.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gxkwdufpw.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gzllbjkrf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/guikgdgvl.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gxijenhep.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gencsmlbh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gxtmrszwt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gyjmgsdol.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gbhoopauz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gjvhuiuxz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gujcqxfhc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghwuekolj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gzwyirtap.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gohfyopdr.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/grknixjij.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/ghwbsitfw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/ggrdzosrp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/guzjiuktc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gdaqbklvb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gzoidybmw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/goqrrmvxq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gvkxffzsg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gkvxmbont.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/ghtqnsdkr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gwrouprbs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gomuekopg.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gcjunbati.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/grpisaene.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gigvfxpvy.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gzdpqccbc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gkktadead.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/ghysyshfk.sHtML


<!-- 参考信息 -->