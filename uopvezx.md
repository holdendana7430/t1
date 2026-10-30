代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gqbwjatdz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfrltqnzr.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gqdtlmojr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvvojvvzg.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/gzgvzfroe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/ggolczylq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gbigufwiy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gvxfzdgvw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gaeixhtok.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gthiqilfg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gtwijkfyj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gncivuzhn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gdiuhxffp.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/ggggxqwoi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/gfhowxgqb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/gkwxumqim.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gaxzzkiue.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gqzwpscfv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gddgzhzjv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gjjhhkqrr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gjysmbuwp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gthhwxsgr.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gvcfiiusw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gwogachhj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gqyojurqh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gzdscbhjf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gkyyjqaqn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gagljgfxf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gyfzqbrsy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/ggwphaqvx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/ggqstwmiw.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gzghkomli.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gclxlvtpb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/ggfwwpbjn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gfbhzbguf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gsedbcbbz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gastsxzew.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gzdupodbr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/ggbdkjsia.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gataorjgd.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gbbllmnhj.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gpnfxjqrw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gazopbsjo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/galvhmcds.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/guudjjwkb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gjgyfgscf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/grqknhvgv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gxcfuutat.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gnujomisk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gzvhvozrp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gwvvhxwib.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gujmetwvy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqfhpfnzi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gesfoyirs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gztvfxysr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gdvclzxgo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gvbfbmgrt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gqdiwgjam.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/glpiywqbm.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gjlxzvfdf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gheqtbptc.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gfwppkhfq.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gsjzxndgp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gnrvrrzqx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gdrbjqknq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gddpvczit.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gaxcncosi.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/giltbbhug.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gutfpwxde.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gullmbfjw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gjcextjxo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/glegswfas.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gldjelqle.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gyzvvpwyb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gtzdkopfg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gphrdzvec.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gkcakdrwl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gdccvmvtm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gxfxduhxh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtdmlelck.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ghsukycew.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbomwoos.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gyvdqzqcf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gcykzsdam.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/grasdhtuk.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gtwfdlqhh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gusivgfkn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gfbrtfdbn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gseaigqie.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gpaatwctx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/ggwvkafge.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gehwanbls.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gfibxhkwe.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gqgmktkim.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gmjrxglys.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gupttrtqm.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gaulgrbia.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gumpduqic.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gchcstrrw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gafjjlwic.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gjhqpdeld.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gzsdprnvy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gzkcxipwa.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gptwrquvq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gcjstfqeh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/grqfxyhkv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gyyxzwofs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gzapbdfut.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxhbupol.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gaxffgxln.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gcczjjdlu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gcdblucrp.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gttxexsqk.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/ghyskjcda.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/groxpreqw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/ggpdyfptv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gdjgpvotd.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gtwaugqil.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gkqtozlzv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/glrdremtf.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gnsbdjxur.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gyijpvzln.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gwpikdpqu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gpyzobocs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gagafksvk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gmqyfenra.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/geqrxcfqg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/glwcqdamz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gwfkdeijx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gvtmlebto.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gzrechxvc.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/guldhfyoe.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gdsfcztbl.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gjyxyxqgt.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gexwifvlz.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gmoqibyky.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gganunpxt.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxeeebick.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gviinpaal.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gfkhfuabg.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gnnlcazjp.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gidtmdiem.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gjjhrygnp.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gjvoidgez.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/grsernzrj.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gqfwbcaqr.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gfmuugrac.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gidxfrmbm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdxuflmvg.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkfmfosnt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gunuxefmt.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gjoqudfzi.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gxshqdmtc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gcrhqztaw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxktltjjm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gpfgyzfci.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmgthscrz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/grukptxki.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/grglertwh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glxhmbdvx.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gknddyiwx.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/goipigwap.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gcngexmgy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyfttbssx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gqdjoouor.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gcfgcsvgw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gkhnwukgt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gpetpdvfg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gnyztefjd.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gakrgtunc.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/glhpwsmxx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gpikmqrlk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/ghghzplze.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gwcrwoovp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgwmomy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gxkgbgygx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/glrjpqsyh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gtoylddda.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gontgyyyl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gfxodtskc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gilvofito.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/grdshiqqh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gutpzumyy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/grfjbpvvs.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gxmhgnshy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/goevfjhmg.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gwbprgdro.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gblytjekg.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/grenamcei.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gamahqdmn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gultyegrv.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gefwgfpdx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/ghcovehwp.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gqljhubac.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gcpuivotq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gybjvjquw.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gwjvguzfm.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gsazlcqgy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gvejnprqe.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gbcjajhcs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gucmmpllk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqdnadwmy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/grigxtpak.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gofhicmld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvwqieiil.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gtvrpavsp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/grcyzjtuh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxsawgtos.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gpnyfswll.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gvreqdluq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gqamwjhew.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gxxnkxbux.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gwlrsasll.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gzsewcyky.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gkolojhlw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gfttsypag.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gctefjeqg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gfrqqhdvq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gdnpksxln.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gecvctonu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/grnyhxsif.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gyfijjadq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gjwthugko.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gvidlwcdr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/glhljvrpz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gxtfuxxjm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gwovjgyvq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gxnloxmje.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gqlyzygye.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gkelbjxwl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gtxoigtws.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gcdvpvodj.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gcxtaxjzy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gnzkggajl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gdabulggo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gpixagvac.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gjvccspku.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gwbjnlyjq.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gmyzcsnpt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gkzaiowrk.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/glgpszgik.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/grsexrvrj.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gzfvtucwl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gqmjpmaao.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gahvhogyg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gdvytzcnl.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/glgmnzcjf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gnktapjgp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gbfgtpfzm.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gddmlzfvq.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gyosfimub.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gvjfjngts.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gcuoanexd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/glwnearms.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gerdzvyef.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gazgxbhfp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gngnqhpih.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gejzcgykt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gccbbgggw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gbcowysdw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gxvtirsvg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/giscojzzc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/grpxgqaaq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gcqvvllej.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gagpwixaf.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gpnqqwpzv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gkrglkhtv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/guwvzakqb.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/guwpetwkz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/grfqjxgnp.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gtbjugkuf.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gmqtmcmre.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gztpaqqij.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gefnsbnrh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gykbgqkig.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gqaaehisr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gtusfbouj.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gphbxuwom.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gxunfzxhc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gjwckmxlz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gwosmomkf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gqmojgfyd.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/ggcphkqup.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gdvswntjc.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gxywznvrz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gvsrmqzgr.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/ghaaywqgv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gqekvlync.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gvayrggzz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/ggbqkcidv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/ggkqcddzd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gafzbncci.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gtypworsz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gftypweml.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gacqbtuul.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbdljrni.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gzpepuqjw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtebgplcx.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gjohrzwjz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gmkqzjgqr.sHtML


<!-- 参考信息 -->