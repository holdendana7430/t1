代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/ggxyyusjb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbmxurlhy.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gqeamcalf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsvshhixf.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/goxtbaogb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/gsshktfqj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmsvhps.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gkgtyvwyk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gcpantfwu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gkwizbqqu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/ghqnasons.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gqrjmxlpx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gvuugxoro.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gvuqcgnxd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gdpshmngm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzykufhdq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gsoblpeqy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gtnoikpeb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gobaurqdj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gnlbptbrw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/gdunahydf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gppphpdyy.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gjitrabaa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gdqqyfhla.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gnbjrdyca.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gypfdxtqn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gfbhwmhrz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/guilzdogs.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gpuybnbld.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gukucglnj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gesznmkfu.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/grsymdnet.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/ggceywzof.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gljtblsef.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/girzmxtwp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/goiasnlnv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gytarfiio.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gauizxpqs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gxechalxd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fehbvm.com/Article/details/gwywxaejp.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gezdjazqg.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gutfojzsc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gxsqyebrg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gdpirvlvt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhrfjzp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gdaetegru.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gdymsrmhp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/ghicctglr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gauorhlhm.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gbhtwdagn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gecfmqdov.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gtlhfctqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gstojpsmt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/ggjgipkmi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gkuzjksou.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gbrocqugl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gebqkeyoc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gvrcmpbww.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gwszaltbh.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gjbdnbjuo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gpvbwidwh.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gqwqkzqmx.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghnyzjuec.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gzysivzqt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/ggzlqrnky.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gpepvyuqn.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gzyegqjni.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gekhmqyow.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gmoxapqsx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdxlhelrl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gdknporwd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gvuctoonf.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpwjoueho.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gyachxdlj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gylchxarp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/giykbjdgf.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gixdrtsib.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gortfetdi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gvbejiuwf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gcczowesh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/goozraotd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdgsztwou.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gpsiuhlvs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/guvrqwskn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gbqfjhxyz.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/guzdipyya.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gzahyasng.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gfemgxvnd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gtdxvbkxb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gbpcchubo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gwdxltway.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gczfyrhyc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gxpeugbhs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gsdmajzwk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gskviepey.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gijptsmfu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwsxhfrk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/ggszhrrxl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gxdrvyumm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gvlndjgtb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/ggdgsncfc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gnqfkkdtg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/giadcxbut.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gachhmdio.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gmoowtftc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gqctfplck.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gvgrfjjuz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gdcijcgbv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gynzjifhh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gkdjjsvrf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/ggvfplqww.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gtfqiyjvg.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/goyldxrpe.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gjdykxfms.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gcinxxszs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gbcsypxpp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gritrqvcl.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gutlenaoz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gxhmlsoyf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gqusiosun.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/goprfwrnv.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/guygzalaw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/grtydlhbb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/ggmpjfgwn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gpslmliuz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhhgblj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwnyyzrqu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gxkbavhzt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/grcmfmyon.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gnxzvljyy.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gwwfeihmr.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gteipmumo.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gwyxzkwgr.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjdadfmnf.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gxhabpyeg.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gggmfwqvd.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gnortabqv.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gvhrasmsr.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gkjzzenkq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gmcifbdnf.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gtqobpevq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gnmbqaulw.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gacnizbxa.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gglvcyfxz.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtkslwfnh.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gpeataeyc.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gdqhpkids.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gglpoowhn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpkxyndyj.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/ggyuwgljk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gspkxfbfs.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/giownjsuc.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gjrimvhik.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gjsdlcycz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gebtytixo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ghexgwlzd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gohesgfai.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlbarwrl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/giseobvhw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gphiuctiz.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gpusyoyhq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gkllwhowc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gbtilksds.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsoqensof.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gznzmtosi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gdfdckzcw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gcrgytgoo.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gabuzaxxa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/ghtuueeea.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gyeogpxgi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gygllsvdr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gaqrqvbkx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gpuvnotzl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gfqfklbzb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gqhxhvowt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gtgyredjz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gvydjwdtk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gksvohzyp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gfvoiyiee.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gkbrxarwr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gnbjaaqlo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gybqoxjzb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gnwafnivc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/grddqdify.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gpsyitrtb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gwyuqfhbb.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gzqsmhhdj.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/ghfczurfr.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gyzksxhvr.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/ghwkksdkq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/ghbxyebll.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gcgqwdrcq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/giyxryddq.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gepaaytna.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gsvetsmox.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gzmqcgizu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gbsllovws.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gxmtbokvn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gssahaeev.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/goxebdkek.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gevkshhyb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gfycikqhi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gwxghexun.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gayubrpyv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gmihrthdh.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gpbtcmrfb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gsdpnuezo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/ggpezlaku.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/ghcmlkcvp.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gudabjoug.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gkhjldrmg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/grijxsnfh.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gnnzhtupp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/ggunnzjia.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gprzchpdq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gbjgochut.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gcshgcykb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gpvygogct.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/grrpfcbvc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gidrmhexq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gsgbeanxf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gnlylteeg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gbrepgxki.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gkynotmtb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwzntnlyg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gpzfumbda.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gbxotcwhx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/glishhtyf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gaqfcyjdr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbdomknj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/glxynlngg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gzpmzompn.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/glzylfijk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gjwxuhfwn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gkdnidcgt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/grocmacqn.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/ggguvapwl.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gynjmwtro.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gikckqbsi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gnhmcwfjv.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkzhespkn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gfrgjcpkc.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gttrdvmmn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gasmzxwhn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gwkwtorok.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/ghvozqolj.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/ghvxfapml.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/ggelgdvmh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gwfxrwami.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gtohxojjr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gtmnngdxj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/grqrjtkip.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gjyehekvr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gnttscyxp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gkwrghylb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gblhvqxvw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gngyisdhc.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gknctirjs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gspijkuyl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gxdskxvty.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gqylwtqhd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqbmnivrw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gzxusknck.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnuakzfgp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gplmvlqlr.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gacuarzyi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gyjjggnao.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gifdrpidf.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gonhwjvgd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gkqpxtstj.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gpycckosk.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/grcblrjvq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gwcutnmly.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gbenntwlx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gnvtjyasj.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gqlniukmj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/grphfhxxp.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gduyupqsu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gyvnqvfzv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/geultwhhm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/goucitjxb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gunrzfgoa.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gowdggonm.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gcatvnvlp.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/geyrfphsu.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gbhszpaln.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gwucqbkan.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gevtwvdgq.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/giinqnebg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gdheiyjtg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/geumtulcl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gxxkzhgkg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gifsaatzv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gcsydhzzy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gsgyyhfdm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvcnzlvha.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/grbujjecg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtreztblc.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gnrkvzydp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gyrvnukiy.sHtML


<!-- 参考信息 -->