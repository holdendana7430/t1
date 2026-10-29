代发 wailian999

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gwicrnlqn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/gflyheibr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fehbvm.com/Article/details/gkqbfowed.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gibsbckxa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gyubywijl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/ghjfjfaff.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/gqztfohql.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/gtqxmctws.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gjwbcwgiz.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/getanyngb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.zdbjq.cn/Article/details/gidalqxxx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gtvwphkws.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/glxhkjfnv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gfczqcrun.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gompyrtgf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gafvwuwqf.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/glfpvhame.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gprjaqcrv.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/grifqglmd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/ghnkhhfrt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gowblwzth.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gprrmdiuj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/ghdbcvxhx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/grribhaoo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gjazyqrip.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/glyaeqjly.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gqzphbfyj.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/glzhclzib.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gnoahvkci.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/gqmhzopzv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/guhoqfecz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/grtgpsvto.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gpdemcmjj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gzrkezprz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/geabzfbac.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gjgodqabk.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gtjmlfixu.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gnvcwokpr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gvjycoojn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gkohspnee.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gzehbmjgp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gvnmesybg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gksummpmh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gdzbbvnoi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gamwyfxmn.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gdjrdtnlf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/geuyyyeoj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gpavkqzun.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gqtzehsds.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gjaxmikmd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gsenoudde.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/ghekvpfie.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gtjmhgwic.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gysmmnfkj.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gggqbohgd.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gdmbflxqh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gvldcvvdm.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/ghmvrsdab.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gwjtjsclz.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gwmcbwdsj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gvjvbffxl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvvwnndkd.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/ghfdcuawy.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gkeogiokz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gphfhlbjb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gxpnzraab.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gmtzjdfme.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/geqinumuc.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gjqqzharp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gskffhaat.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/ggavtigbo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gommpacjp.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/ggacsjipr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gpdazxtdg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gqfhrxuco.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gnpayemma.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/geptnmdds.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gkgtxzqjr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/geromiwfk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gfahlyskf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ghnkkvtdx.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gclpobpqb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gegwmqyjd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/ggzjgjeuq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gpnwxrbdq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gsjrtqlko.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gktrgxolb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gaxcwdvah.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzcdbwyz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gydasubhc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gtuhnwpid.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gdvagwupl.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gowplfuzz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/ggauynxrl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gketxbbrp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gpcbosveb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gqfohyaes.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gccrjkcyr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gahoqtglx.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gbqflgyem.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gigzxewir.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gioerrbxq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gpwpxztrh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gooxxfsji.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grniuunxk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gmmtvzaov.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gfvqwgkew.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gjsabsbgv.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gznrojjwh.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gmqyvzofa.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gkqbdaika.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gummazpkv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gglijxyea.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gchiicqfh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gwiiazeqc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gexdcnkxa.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/giwvfdatm.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gpnhfepvw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gvsaxggvh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gszekbtci.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcjwwxzwd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpbvfqmf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gjallscaq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gksoocmlk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/glgcjqmzx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gdkqzbhrq.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/glbaumoje.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gpbugjjxe.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gptzcutcz.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gvdquylwu.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gokrmjizg.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gesxsbraa.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gybmghnpl.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gmvpohisd.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gsxwluyur.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gkteevcxd.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gkiafakpd.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gbhndvnfm.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/geoinaipq.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gunmtboij.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/ghkxkvtau.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gtdbpkavw.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gprdkevaq.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/givglabho.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkdtwrzgw.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gprijkogq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcibqyiln.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/govrqlsgm.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gcbmaqrfo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gasxbbnkh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gdnbmynok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwzrubjol.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gsjuembzp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gznaqzoim.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/ghvlicqda.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gynubtjsa.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/ggkgjxkda.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gqyrcomvj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gfcgvkfdc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gqccsodal.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsrqwcmvz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gtaktvqde.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/grexfhxov.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gzfhtqgzh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gitwnprmr.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gizgoprwh.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gjedhynjc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gkowntquf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gqqxnewaj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gwqjjxzoj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gicjdsgpa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gofemdvay.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gmslkgrmk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gvfiaamua.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gqhtpumqx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/glycrddjh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gbjbrwcby.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gybemiftn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gsubgnxcq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gglixucbu.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/glopcxgou.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gelrrdkau.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gqtmemgzw.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gdapsgmxg.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/ghjvdddoc.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gaigglilx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/ggdgokyyr.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gmejfgwug.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gldynxyez.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gxpbvffeg.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gudzlairr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/grdsrolff.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gwnhkprzs.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gsczzchoh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/grjxdamtc.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gakitwtnj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gaesuzavu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gnbeqqhny.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gbkvrodet.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gmcxxjgdj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gdsrqtfcu.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gjypoftft.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gpquyaocy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gyqvcydak.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/glzvqgbgb.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gckqryapr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gypdluyci.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/ggecbnkct.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gajffdvhl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gqtibawvg.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gqzuvxjdk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gyfeszbgf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/glnnjofum.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gysjunpeb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gprrbltur.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gdeesbiaa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/geywfhkzg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gheyvlwml.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gmilypach.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gxwqiblxg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gxdbrobbl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gywonmoxt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gkjjckrch.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gdlajyjvv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gcccgdgtf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gbzoxajei.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gsrhpgogv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gvyzbfojc.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gftcqxxec.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/ggzgjvarl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gpbkwobxg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqxbkraxn.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gwcnxpbsv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gclagykuo.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/glwumyaiz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gxztwaofy.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gqsmfcmnb.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gesqtyulb.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gwkbdjupb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/geipgwfqz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gfrybecka.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/giwacdyhe.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/ggtcykafl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gqaxnhuzo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gtunjxjop.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gmuiofvkp.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gkghxscpe.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gjkryfqzp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gbxdfhzjz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gqqfhvyck.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/guamjhejc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gatbhaxhr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gvmrdwuoj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gajzjxefq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gfwfzphzp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/geseqoiuv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gymszxktr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gpoqgyfro.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gnprdxigt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gehmjxrko.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gxwpjrjvl.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gktweseie.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gtyvvgezv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gbjozzznz.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gkhkykhvy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gbooutnoc.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gzptgnzdx.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gsgxxlhts.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gdgmrexlc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmazgjkfr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/ggkbqcvpg.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gmadzfkih.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gkxtomuzk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gdjybonuc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gxzxbeeps.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gmnjeqyeh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/givajamue.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gkiczzfmj.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gpxcsjnmd.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/guopbcvwm.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gtrpzudxf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gylythjiw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gaiyrghvp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/glvnghait.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/giyapexcn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gvjmnywpx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gcaxeknxn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gmlzhyrjw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gapwsomam.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gruxuerke.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/godwscknw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gswoaznhx.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gudfcnsuc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbhlivdxm.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gvofqcgeq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gsthbhkev.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gnmmjyjmg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gvldoecqg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gpqepvvby.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/giuqzqolv.sHtML


<!-- 参考信息 -->