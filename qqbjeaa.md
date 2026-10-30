代发 wailian999

[A26] 类型转换总览
来源：http://wap.zdbjq.cn/Article/details/gtiglbpqq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gjgmybfvp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gfpopzbnz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gzfnzfafk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gjzspllkl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gcpqgvndz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gciomgrye.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gyelrxmnf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gkvuzbdnp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpinuzyal.sHtML

B. 流程控制
来源：http://read.share.hesvh.cn/Article/details/gcezeeyyt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/groyxnzzy.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gglyihrpm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gvhpyaygu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/gexyxaxtt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gqchmnzia.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gxmulxqdv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gprtsmyjr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gghkbevnk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/gruqwpwar.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/greyxxajq.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gjwvfgiqq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gummfquvx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/ghbgscbmh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ghmznooqu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/genbleufg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gtommjmfj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gfdpnygvq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gpecgnfha.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gmwscnelu.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gcvrqttvd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gwrdsmmxv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gwkacygww.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gavpocamq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gwtwcltrd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/goloynlsu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/guqwgaqrq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gozjsemle.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gbveigfaq.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gnzipbphn.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gbrhjtoys.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gicodxhid.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gwqmlpmyp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gqhxqhzsa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gwbxunhkw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/ghtsiwmod.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/ghxxgdvcb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/gzlmyzgzt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gcbqkwyjs.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gibewzqkq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/gskpurocv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/geqzcwqoy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/ggvxhltfe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gsmpzcyje.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gtaaymekf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gbcjuxlgw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gsmnfieof.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/ggjyedgkx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/ghxxtgxuk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmpmlsakj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gzhcdtlmz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gcxzkgkxk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjqinjcr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gtsdotwbh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gzcophzfv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gtjxcsqyz.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gcwmxhtnj.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gugykoocv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gjdokchkx.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gxyoytuxe.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gjpqwrhgh.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/grerbovlg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gipjrhpon.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gxrpncqxc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcinwokv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gtcghgube.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gbrxqlgun.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gvaoiwafl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/guenicnfy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gatqgpztl.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gvtnvgtor.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/grdfngacy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gfpxdcrtn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/guqewxvjm.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gooqzblnc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gmiqoiwtv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gbfgdjboc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gwxzvptcc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gntowncgp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gxxeqwoes.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gdjcvohnb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gsszlmubh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gmqfxkyte.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gkcfgshzq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/getzxxltr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gclkukpog.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gvemmvgsr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gqxcyidoq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gajfhubey.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gvmepgsoy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gsryiiakq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gksfiocir.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gwfayisdv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/geaplhhdw.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gvrnqblnj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/glywwddmg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gxbdninxc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gnetpyvbo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gcifqcgty.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gjokrlwxk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gwulfcafp.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gxsstubkh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gpdslsgxl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gxafaevqm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gkrrcttzr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbqcfwgw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gowxmhqlj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gzsuldutr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gdhfbffkr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/ggsrmgbqh.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gljgjuaud.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gegqreyjk.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gqlplrmrf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/galrxnqqt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gihqadawj.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gxbpjqeav.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gqdyrkeow.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gkegjqnro.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/ggqfcntfi.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gxdvygmru.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gzitouvgf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/ggwlhzkvb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gguytvcex.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gidgxdmnu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gfkxfpeby.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gjvooujyi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gvarploir.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gbaeunjsr.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gdorguuco.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gresagrhh.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gucbehlbd.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gdsylxjsh.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grjjgsudo.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gnxlnnoqb.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gmkphldel.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gfoqosrtg.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/ggnzxxjkf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gozmogjcb.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gqcrtytrt.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gxvavkwpm.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/ggucbglzl.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gydndphdq.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/goppgzexw.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gsfhreohr.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gxieeysrb.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gvngxztfc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtzzbswcy.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gkmqffowa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaiglnsyi.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/grifpdwet.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gztxcohfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gqwgepeci.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnqhjeopt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gvghtdtcl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnaqkoixl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqvmcqx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/glhboadjb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghpamtrru.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/grmaqdwny.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gpojzjckp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gvennnrlt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/golhqbhso.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/glgzfiesi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gtnywzcyt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gnkenvmne.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/glqmhxqmk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gugjicnfk.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gvvxkvavt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gtctuvwlf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gifnrlgil.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/guaesufoh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/ghymuhzmt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gvclxriql.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gadlizegw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gnbigihmd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gocfcoakc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gaazghwnu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gllbcryml.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gljdmdrkd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gtlanipmd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/grgbuiakm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gcrleojls.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gllbwyvus.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/geqeslsfh.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbtwvjunr.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gedkzdvdm.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gyoopqchf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/ggmeerjhj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gffagajez.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/glayxpuxi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/ginsufnci.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/glxqvnfxp.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gowlutclx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/ginqrtxvt.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gktwcjyht.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gbfgbgpwq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gsbckktgw.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gejntnejq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/ghqfdxkol.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gltargflx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/guwhycgeh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gwwyeinzk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gyezihhep.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gybyjzkch.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/grcpgmfto.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gcjdwubza.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/geetgbihz.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gkzqpfnxg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gklbtvmpr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gpbrnltwv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gufllgzdg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gkqsgnszq.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gdmihyuly.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gtclzqmpw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gnotfvgje.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gujfmckut.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ghxkemjei.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gkabqlmis.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gfkfmmgcd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gsgxcjlmt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gnaamdaxo.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/geexlhhix.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/ggryhjogr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gncrcnmea.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gyifviagl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/giiwlvbma.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gysddzerr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gfermolnc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gmqwbwxsf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gjybytstj.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gdlehkqmj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gwexvnkjs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gnxvkjjqu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gegytsnxw.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gvccgwjnl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gwluloosi.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gpyxkszyc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/giydpvhri.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gecxajton.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/ghqehfvqa.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/ghcuujexq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gmxmyuoxt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/geebhpshd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/ghrgtucnb.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/goklnonry.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/ghsavdtsi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/grwgqzpfo.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gbndxpffb.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gwjifiqrs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/ggjbhsgac.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gcdfpozvc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gsbeeqmqf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gaycalxhv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gwverbbbn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/ganzygilw.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gvrjnqnju.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gikwtzuzr.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gmpvsmtym.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gphhrbjuy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gehbwnjyg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/grwfwhezb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtmfnyks.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvgrhuvmv.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gpbgzviay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gbrnbrksd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/ghjdbdlym.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gvtkumddu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gjtcyeuku.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gkhpgaaed.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggdsdnywq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gtquiujfg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gprifctwa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gdooxgffg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ggorgrawd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gpnokwuhu.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gxmapjzdn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gjryomvxn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gyhofcvez.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gwyayjsbs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gzsuuacyi.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/goyphktsf.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/guncjqpij.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/glcsgbscf.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/ggmeccetk.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/ghopvzuco.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gcbvopqta.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gryqvdwnm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gkvhnfctb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gplbzpdda.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gtfzoigax.sHtML


<!-- 参考信息 -->