代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gafocpgvz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfoxwceqo.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gyqfewjrq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjiqnqood.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gmrhxbjva.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fehbvm.com/Article/details/ggkuuzsnc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/geadahcwu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gsdwtauta.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gqikndzeb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gepzqsivm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fehbvm.com/Article/details/gaevdxmrz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gwmoddzzf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/guvrhcboc.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gnddujgjl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gvonodqkf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gixpmicio.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gggpnywsa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/ggnupfpoj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gsaatsudf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gddrbqbyl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gmoeohapy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gxwxjglkq.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/glzbvxcfw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gcienuckg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gwmgkthgw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gzeopzyda.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/ggyhpuvlo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjssmffjr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gxtgonwyy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gowkmjqte.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/godpwmtsu.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gplfdhncr.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/glcchbtgz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gzpukgckh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gnjbvnwwa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/goquojksd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gmcribwbt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gidbrqfdj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gxncbhonk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gjvxbykpw.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/ggssuczgo.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gqphkygld.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gwjvcswql.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gfeidbwzi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gibwsnlzt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gwbsxjalm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gnzsklosk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gwkymhayc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/grgzkobpg.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gwuiolyga.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gqzhhckxh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gsndmnzum.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnyhbkdb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gsqihtkzc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gdphsqdxt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gyiaanulc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/glmknvuly.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gwlcpwshz.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwnsyzrps.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gknovuzoq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gburzhzcw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gflowjvsd.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/ggordzxtl.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gyazcguec.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gljuusxqq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/ggwpxcsfj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/grcgiunae.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gkoysifuv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gtgmksisu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gxnntrlhy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gnikrnkiw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gpbklyjsw.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gcpsycmby.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/govvdqnfh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gairgxyna.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnecqixef.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gygitjnbt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/grujfhcxe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ggkwhrrgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gfcnedxmm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gsqfdkvop.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gvvtpbskp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/girxbyhkc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gtpfsoclh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gjqcvojpg.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gvitczdiz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtltphzd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gibbtmfhj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gpcsxbawb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/glnxvijsb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gnniwbksm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gituztkji.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gdftnbote.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gvkqkwoub.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/ggqobdhwp.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gbkrjmdya.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gvyyblamq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gnlryvtai.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/ghycpmrkt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gsgbnyzvl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gojdxisvk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/ggmnkuduz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdyhowwdp.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/giosfskxw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gxbbkwrmc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gteqlxfdx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/grfisaxjf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gtdjyxsuq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/giuzhcwwc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gkpadfoik.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gvtylpiih.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gmqegufdv.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/glirsvwrv.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gwddnvqah.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gunhmyigc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gzprinmbi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/geoovbwqh.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gmsdsfrjk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gvjnrhwmp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gobsvewcw.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gmoooxpji.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gkwuhgwtz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gktylnpgg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gyqfjigmk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghyvwzbxb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gdfawmoml.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggpyuccpf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnamvofqg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/guojsglrm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gzhduloip.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gbpsmgxtj.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gdwnknadw.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gxzwswbzm.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gmnpeyldc.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gnbwgqpsu.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gwhmxiwlp.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gfzrzmrfe.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ghbbfavph.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/goznbflcy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gweiaqgze.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gqclugkan.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gqzuyubuq.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gvznbjifo.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gixqwxntz.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gehujtdpl.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gjviwzitq.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gtignraed.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gvfscsvzo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdaidkrph.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghafbsvbm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdrqmeymp.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gvvaefltt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gstikbjuf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwewmvfmt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grdwmywzj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gaoahvtfa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gczttmyat.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gyizhtmxo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/grcxrjxut.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkcskarly.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gsgrdnemp.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gudzxdfro.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gvrstmgsi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/ghzegivop.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gwajoerlb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gsmafvrcl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gsvwxyxhf.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gsrwgflmc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gwfnpqrji.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/guvrqpcmv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gatwrnnjr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gshbsjmmx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gbvatskyl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gwcoatxwt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gsfnwohpe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gkhtpblti.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gtstzqlnt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gxtregsgs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gsdahycuv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gbyqyyhwe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ghzbhgrgl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gesadyank.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/giiqxmaod.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gsyqlpvlq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gesodulxy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gxyskmpst.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gurjekask.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gvukfnaow.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gyixfpydl.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/ggjzsbfgn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gslhjyqkj.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gwfhyrzbs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gltailzcx.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gmkqmvszl.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/grmirarbq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gfprpvdsm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gevnjmzgh.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gesrixqgd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gvqnsqcwr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gwpanegmn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gjntyphnm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/ggrnvouot.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gyeuwnfgl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gmzqzybpj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gwnlqenld.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gnttltybt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/grqyflejz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/ghafsfjhl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gpjqwpxzn.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/ganzpcwsh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gttmmjvja.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gjwebbqqi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gohxkbfbj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gwquexijh.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gntnsmclp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gfjsbjuxb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gckkmypfo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gxkgoesuu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ghcabeqcp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gtaqskryy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gxhnykxdx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gklpkxihs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gnwbfythm.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gwsixcuon.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gvehvwgge.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gpaasdiqs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gcbvzyjup.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/ggsskffpi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/grlayhbgq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gsqvymrqd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gvjpxpsuw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gybompdit.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/guatycvak.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gwzckccta.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gohksawss.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/grndffjcr.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gzwscyppy.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gchfokuza.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gachqtpoz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gzqajykjv.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/giinvoofi.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gecxecrch.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gifqutyvg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gjexhqtrs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gtbpfwlno.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gsqupmeva.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/guwbbftkv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gjnrocykn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gmvtnirye.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/grikpnnjd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gfnwkuygd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gggklzvdu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gvfzmtmor.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gytrpqpat.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gcnmjjfcq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gtbmilrxg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gwxglpazw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/ghjqgogwf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxmdxvlgb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/ggxifulip.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gxsqremaz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhkzjmna.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gwejmisey.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjjbyomhe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gbrmhlgdb.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gdacpdjch.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gtrhnxdru.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/ggfsowjud.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gzrwcwyle.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gntdnqrvv.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gzqwhpicd.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gcsdopmcp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/grheymvug.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/ghikviqge.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gulzgpdfd.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/grhkmfdxz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gvwtombod.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gbwymdspw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gkufchlip.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gblzgqbiy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gyxiwcate.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gghwcsnaa.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gttpvnwuw.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gicexzhtn.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/goyykncdq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gzuoizhdo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/glonolcrd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gxcinrwpu.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/glpbgpaim.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gmjligzxz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gakelojyo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbozblxjk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gbiyyrgcp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gylujpdot.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/grxuvnbkr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvlensvc.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gvyeasaca.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goejvvvpx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gdvrnryia.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/glnpxgtxe.sHtML


<!-- 参考信息 -->