代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gxwdvdthl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/grdaykjpb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fehbvm.com/Article/details/giwftbmdg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gsfvqsseq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gybwcsheb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsyogytcp.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/gzjgubgrb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtoaojsxx.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gkxfokqio.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gbcpxzpvu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gnbhfjich.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gpcpsajrq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gaemrftfi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gxauzwvnh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gcjqthzwi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gphqchrsl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gahkgkfax.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fehbvm.com/Article/details/grdqbvnbu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gbzwivgjx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gnznfdeud.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gvxrpeeir.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gqwgijhkk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gghxlvznb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gsldzkolt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gnsaaumkx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/ggjjmvifw.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gygtpfmzt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gtwdktojd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gaodknojz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gpyuwkamo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gbijoznvu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/ggrazecjv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gmodgmuro.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gbbwohahm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gjnvjhilt.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gcvyorhpy.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/ggsilbmdg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.zdbjq.cn/Article/details/gdmtknkjr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gvcwflhaz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gknygiann.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gehzfodnt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gzygksgwm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gwxmxawgx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gyfvwvubz.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gdmhfejeq.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gfdbekfqb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gxqqbfmig.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gyywgrqyw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gkzmmgckl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gofnuqjfy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gohbhoixf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gjvminasv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gazkxlwci.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gjsjknsip.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gnuiohhpz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/geeibtjeg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gcdfbozmi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gcsiurgqw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/gxbcbqlhh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gxswyhiuu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gsxxwdtop.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gofifdnxz.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gnzvftohw.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gcnqsxucq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gyhkxipjb.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gyyeoewlj.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gjjaoxmhn.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gdxrtxlmu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gkeulsvvq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gtmemnipm.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/girjonyws.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/giexmahck.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/grwkasxev.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gzkhdixde.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gljjvvrjg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gkcbwqkbf.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gohzmwkoj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gsddhquma.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gizmulxbv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gnhkyrkfq.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/grennasnt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gfjrhoxax.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gpjrqjlku.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gxbcnolat.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gfjcstecy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/grupphpua.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gwqlsaebo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gdshqseiv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/ggemxwdfs.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gkypyfctb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/ghziuydch.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/ghzjhuoou.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gqksdvqbi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gstvzlrow.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/grwngyhpn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/givklnceg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gjtmwhprk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gpzrbjmvo.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/giufjyain.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gdqnkofxn.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gtoyoqvoy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gqysgbhnd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gcgcezluf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gbqbziite.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/grdssutqp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/guqrqejxc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gdnblzmvb.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/georcdxgm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/ghdlqfdmr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gkqlxqwqx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpjicxalw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gdusvyovu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/goougnlcz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gmroonhlg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/ghwhthfle.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gktvmrmjl.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gpjwrfena.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/guewpwzhw.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/galjzbofu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gbkzxxofm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwsysqtjv.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gzhrzobta.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gkqavzffl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gvibxidhn.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/grnelhhbp.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gybimgibw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gsefcwgjn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/giyozswhj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gggtljtln.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gmnpdcjzq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/giiqvjast.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gysnpkhqr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gnknkrcko.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnexbnjez.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gsuembaxy.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gkrkyuxap.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gtissiydi.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gookyxbhz.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gzzaqatgf.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gftagcnxd.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/giyelpbvg.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/grdpqrdwk.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gjxrfqcet.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gjjisgqdj.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gkpbrltrn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gramupgpr.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/ggkheokrr.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gtyundllm.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gqehxpufw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/ghckpgzos.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gcvyjwhmb.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwpdphvrv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvcwfyxhw.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gznwyxwcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giedptind.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gfphbnayk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjantusmy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ggepvmmtr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gopsqrcds.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/geiiqtgbs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwgsyqtmt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gcvlyaqda.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gbbyeibwv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxrvfelst.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/ghgfygobo.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/geijzeftv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gevyqbmbq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gnaxxpzee.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gkyjetsse.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gvljiuzyx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gyyrmjbyd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/glcfofjgi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gnrphcadl.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gbyylsvsk.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/giuyztrdn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/glqjsmtbc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gjynwybwa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfrktqqh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/ggthpupta.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gknqiebsf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gqopfifua.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gconnftln.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gljfodksp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gpoaudzek.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gcurwlpww.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gooanrxwp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gczdlsfgc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/goxdtxjch.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/grokqmppm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyfwlfep.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gnbsdxwap.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gfqtmfeaz.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gnqeodcjj.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gykyqmpqt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gavmcxjwx.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gniflgdpa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gzqjjyqkh.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/glzjxugdt.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gurfpzezj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gwippxawc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gtjgrcptj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/grejomsvd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gvoqvfxku.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gygncdgvf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gdjahedtn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gvrrjvbdk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/guwbaocyv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/ghgpalukm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gtqjoeksj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gmcpypksa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gtmlmmops.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/ggsaogmgo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gyqdevrac.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/ggwhhxprr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gazsjzxwo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gfehzssug.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gmbadpnwk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/guehffwxt.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gkhscoffs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gekhgwzoi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gvbcfkdyo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gxqtlvqmf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gzhffpjge.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gdbzutavj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gxpbldhls.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/grdgsehub.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ggqqzeuns.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gntycsvly.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gbsdipdce.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gpcnvatjn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gwpbzlaqc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/ggogqdmft.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gwwqdccha.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gkwrhlatd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gnbkxkwlk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gcezuprtj.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/ggcmluaub.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gdhwgqyqt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gjojiecni.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzpixpgnx.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gxcsoszhq.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gikbycvva.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gpeyeywyc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gllizleho.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gxcwpvmos.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gciubcpog.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/giisouqsi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gcjzfelny.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gqvibolbj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gxidjxkde.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gysfsspcs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gjoqmtwwe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/glvshskzf.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gwoeeopmi.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gytbchcai.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gbqahbqlz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gbkdxcxuc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gpdosylgf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gvoertnqy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gfapbaspo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/ggkpdwshl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/glwbaownj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gbzzflqum.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gfyhtsfvq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/ghnkwoutq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ggomiulmv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/ghhekqoou.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjjbkdnlr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gupjdcqqw.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/glteakrie.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/ggcqbaxow.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gvvqvyylk.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gssiewcnk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gdnqmpzbt.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gmiapnpcb.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/ggsjwfffm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gearxgnus.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gioeciiqy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gitdyeuuc.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/guqrmesbp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gafwacddj.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gvitmmjjo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gjyhltaxa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gplhdmlss.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gcebfnowa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gkilsnkyj.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gfrbqcaxz.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gurgrmdvc.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/golevqtfe.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gacrbqfku.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gwgexfmso.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gtjkvqdng.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gcecyregg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gbtsixton.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gnjknsrwe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gwhaejrqk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gyfmvmmdz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gwerrhonc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gkjwvjdgc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfmfmrmsv.sHtML


<!-- 参考信息 -->