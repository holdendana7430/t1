代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gvizwlmza.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/gsolwisgk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/glqdjupiy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gukhnnqju.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/glxklisxv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gnbtzrjxr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/ghismqdak.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fehbvm.com/Article/details/gudjbbjno.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gubiubyag.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gsmryvxrl.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/gbtgtkyya.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gretysqoe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gnabngwgn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gvxvcmgkg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/ggsvkmvxp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjwyfdqvq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gudettlzh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/ghkzohdpf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/gsrwbaqwl.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gtqvgzqui.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/ggnbobmdz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/gmxmfzkur.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gxfdgbrfa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gvsbjchjz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/grexssgeg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/gewooolab.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gjxlsrlbd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/ghspvrsvj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ggeocijvq.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gegsrfnqo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjexzken.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gnwuwmctq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyiyrjntk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gfeixhemg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/guuuojzgv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/gfjustryt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gkgfyycoh.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gzccmxvwc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gvqioackh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gmecxcjmv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gnopcpyze.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gjngkvcpu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gftrcxfhr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gvxfvhoey.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/ggkujfibu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gzablqfgb.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gfufirqke.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gmzbnfxoe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gkrafzmzh.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gcqmejmvx.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gvjussvhj.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/ghaprofvt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gfnwwjdtk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbufmzzhg.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghktrqmik.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/goikesrbc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gsppaymao.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/ghqbxllnh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gsucyegta.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gbpbecgco.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gutwrpqgt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/ggqfjexsf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gqswcnlcs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/goibpdjio.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gbyirnnyf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gowkpiwmj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gtzwjsfmw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/girlqvjvn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gocuacviu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gvusddccc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/ggtarfrfm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmopxyslo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/guozzaapy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gvbtoufci.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gjdaalhcd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpsesxbex.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gkgxokkxr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gqeykkaki.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gpijlcazg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gevxcwhvm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbheutnjj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmslpeljl.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/guaezwjxw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gwesgifio.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gepteercb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gdslobyjc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gwisquanf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gunkrpvos.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/glbibbbse.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/goxftaqif.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gthciaigd.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gvdplzwre.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gqooskodw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gepswaczu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gsudwjsff.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gqcworpyn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gxukdlkxr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gxlloldvm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gcgqztjjq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gsndbmalx.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gkhnusaxl.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gokdkaeuz.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gibnbwmcc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gtynoevdx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gevziymkn.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gjsodheor.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gimtysgtj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gmqjqupzq.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gszzguknv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gzikwrkld.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/grzqvgqze.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gdsxqvxvi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gohnulcmx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gnsqngivl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gcndfjqyv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gfcypfyfg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gbmtdondh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gflhmjlbj.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gjkymnbxc.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gwfyqikbk.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gyfaldati.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/geujvzwwb.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gpqwmcqap.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/galnpqghx.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gagsudujn.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gzmdyqegx.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkqrusife.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gfxxftooi.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gscoyrcod.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gwdknnwtn.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/grbbrfggh.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gdglfhcve.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/glttuvget.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gqxkxdeoy.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/ggxxhwumd.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gftwwyxhk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gluqmwxrz.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gzzannkbu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggqshgrod.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/genykavxo.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/ggopwsfzy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gyeuxdwzh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/glskmpfkk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/guohujpxw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmlhsfkub.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gfffzyidv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gorqdllao.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gvpiphkht.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gmhnlotpa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gjqutzfpv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gvylmafsj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnndjdazf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxyfeklou.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gkuehfvvk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gnnzosfhb.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/girvvjfhz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/grgwoenwj.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/govsvfjfg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/ghtihwcpp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gkkzfstwx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gxmsmsqos.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/ggftjunvl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gykctuthb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gqgwdsrag.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gphcnxvzs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gxsfxjdmp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gabfrbwqf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gqrizgdma.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gftitsbzn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmelidiqh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gcqhsioxx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gqmslccmf.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gjoprmier.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gjqqlvzpl.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gvudtvfix.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gxpgxddtm.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gympdftrv.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gurgalkxx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gimwdwqnb.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gwnuqznla.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gbhiqaqvm.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/glsrilykz.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gwotpjtgv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gsbgpljlw.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gwzyjsklv.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gigzoygds.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gdyluucrt.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gfpnaoait.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/glwueafql.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gudrqcdua.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/ghztkoesz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gaesftflr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gfqlnhvih.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gswazbwdo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gjdhoxrkj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxubipjz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/givwanvdn.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gjjzsjqmh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/grdxkyogj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/glaxpqpqx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gtrbwjmsc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/glutmkqic.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gxdazjazz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/glvatfjvq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gcgsztlwh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gxvioolos.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gtvnrcdqa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gzmkkchmd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/geoxejhdp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gzlsugmeu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gefxxxuax.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gjyozpgkg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gpzkqizya.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/ghuflnyzh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gcjfigjgy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gwsqnkjrw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gxiepkmpc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gwnumcmhk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/ggslukgmd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gzguoynvi.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gbdrbrvqx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gevcsqtnp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gbpniumyc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/glsocvrwk.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gsuxpzkir.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gsbaxniuy.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gnbydyjrc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gdylthngv.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gblzdrtjp.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gxzijusgy.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gzhncsslm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gtxnjcsvy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/geflnkifp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/giggadimf.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gpcxucgwv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gudcgcfbc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/ghifbwzrr.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gqieztpls.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gwacyvdko.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gbvnlxyzy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gwzbzzdym.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gjkuhxnsj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gvirzeaig.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gzcjmjjac.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gxivsmwpb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/glsanurao.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gxgkvdvqz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gcamilnui.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gasabhstj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gurcujvum.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gxbdtvwyo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkadkcrrw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsulzpdmj.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gbacolpqx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gogezbjet.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gdhkmdaqd.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/goupghsaw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gtmywstey.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gnambqfgz.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gnntbwjdf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggkbphexu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gkldtlgel.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/grariogxs.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gjmatstgd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gndkjrvnt.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/ghmkxngio.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gvmmpdaks.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gqnvdfoeq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gdafipunm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gojraixfk.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gefpjkoqw.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gjufvxlfw.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/grkoddoln.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gmnihuavr.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/guiabhkdr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gkxthasma.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gxsidlbez.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gngmaojgh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gvtjeqxhg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/glckmpxdx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gvbejdjgf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gvmpgdwyz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/ggxxhmsbc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwcwymqdu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gmhaujgqs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gazmymguz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gvmzstrzg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/grhkyycke.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gaolotjks.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gibyuzyqb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gqcctlsdh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gzenezxox.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gkuwmlezt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gbxjiokmn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gifxikaga.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gqeyaxlma.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gmevwqruj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/grzaxbxvo.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/grbisfxxb.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gbbhybpbw.sHtML


<!-- 参考信息 -->