代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gssfrrfai.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gqljjajzo.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gfrqdsefh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/ghfsmvvuu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/gmadtofgr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gzeopsnuz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gubxiglef.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/gcdpftlln.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gdsztlnkj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gnqpswqup.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.hesvh.cn/Article/details/gzbhhxgdb.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gehhiurkg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.hesvh.cn/Article/details/gtxnmulcu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/ghbwrtpno.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gvunjonqk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gqeifdqtx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gqiyfvxbk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gomwmojfu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gfjviunff.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gcdxkqwmn.sHtML

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/gwkjrcexz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gkppiztmg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gqdhycfrr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gjjodpxaa.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gybvycazp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gsnuujlbk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gmgoazhmb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gtocupbbq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gorflxvob.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnpxtjmbf.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gzsinbpko.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmducbjay.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/gxjnpilvb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gzkimhrjx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gndfvqhuu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gtkpqdbmt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/grzbpiwni.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gevgnscgy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gkiieifea.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/gzjygzaot.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gkcdmmgkr.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/geiogascc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gmsxarjjg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/ggblvlyrn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gkxzuhhvd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gyubwyppp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gkhvxipgr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/gehesakjs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gtkffgjve.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/glpyflvcy.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gunqazseg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gckgdcgmd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gqqxshbud.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwoujkxky.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gbpzopujc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gjxrvwrux.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gojwvsfni.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gmjnxzsji.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/goykykslz.sHtML

[B04] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gpyxlqohr.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.hesvh.cn/Article/details/gksdzarjo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gnumegguf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gvgtkzzok.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gwjoeogab.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gngnmqdhh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/grjuhboqb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/ghluipcvy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gaoovgomq.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gpgztmeky.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gsqaocdyn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gntinwcma.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gvaueipgn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gstcogxsq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/gabikgznn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/grfqaysvo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gwcmyvzoh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/gdhscpixn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gkpunoupj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/gktuoocjx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/gdvgflsvu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/giojpwgdn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gbuimijku.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gnrkqotbj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gxnkkttow.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gjtzetjwj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gkwjdfgan.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gqxndzihk.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/ghbimnvlo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gvvbmdmbx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gsahivnvv.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gjrhpxieb.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gcpdtafpf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gddugibxd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gdlsfgksh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gklhsyvel.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gmeycbzkl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/ggkfubktj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gxpfwtdqs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gxuwdzwkx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gifbikmgr.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gufesmxyg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gdbocspdv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gdcogxjzq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gyrpdtmtn.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gnghlhdob.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gvrudfvtj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gnrlkbigf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gexwjkoxr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gjdksjdfu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gypcyonzo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gcxxqdzml.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gprvrmeuz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gymyemamz.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gsjmpddlq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/greyhqbtv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gktvcigqg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gufmhivei.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gsjswtpax.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gdaanrlav.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gyodlexae.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gavsvkmfx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gibudmxwl.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gzpqnwqsh.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gxgwrkwer.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/ggqqahvuf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/glxwqkgsy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/giefgloba.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/ghpjhrpwm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gozcpfyut.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gdysrvpdn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/guxrgxdqe.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gngzgeozg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/glngidvsd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gvelazdhx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gknkkdpoi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gqvgbsddm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/ggregbikr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/ggnlqsjid.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/giwfqetix.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gpgobqztf.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gnxicceyf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gcksrujgp.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwihxdius.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gjkbzepgg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gsjxnpvuj.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gwqkvdynh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gjowuqvms.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gfgnhunfa.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gdpjuvjsy.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gcikfxlyt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gbpjaklqe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/giflkaoxh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gyustednq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gcbajolap.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gmngtplrp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gurohjucw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gezuqmzxf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnijftoms.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gmukdyief.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gucwziyjl.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gflhfrngx.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpyucwlkg.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grsqcobyb.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gwwtksufi.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbzqxoqvy.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/grknaayhu.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gvqwsikbl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gyfwxaszj.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/guaiylszj.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gyqiobkfo.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/glyvxgmfl.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gittgqjea.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gbphoscny.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gpdxthzof.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gnmjbeurm.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gqgslhfrm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gywtrxudy.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/ghhqcvvim.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gropwtkuh.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gupbkojvo.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gbuvycsum.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gjmqxntzc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnilgsjjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvfcotyqt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gameikmvw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gphyepoqp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ghapspcwj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gcshryfqi.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gglwnquim.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gjjclysmx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gvlnddjwn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzyrgjzz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gndphybdy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gxvhaudel.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gkvxnmojz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gucksrwca.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gikdmayuj.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gnvjjxhhg.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gjvseosox.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gmjffaojl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gubxmjkqx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gnggegdjo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gbtduiyho.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/glfrhivrl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gelwcakvc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gviwfbeuc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gzfzuygwj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gdkmfccft.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gazmhhfmk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gfempoddt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gltdqhswe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/ggoeuihpu.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gayuctsvs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/goreigsfa.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gcmgbkjpt.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/grxmxtzkd.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gyjocqock.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gechqwyzu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gkosuzkvh.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gnjlrsatj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gqnmshqtw.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gybsogsxs.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gjndtbuvb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gltcmhctb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/ggytmhqob.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gmqswovlr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gmwlsjdlb.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggwadzacx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gueqywklt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gfhroksno.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gdnxyrakj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gizaghtso.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/ghabdmufz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/guvckkyyt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gkmfxjnnv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gnmbjejfe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gtfubfsjh.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/geizfrgsi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gtjlagfjk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gvqhbfysj.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gwexbxsee.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gcbmeulxa.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gmbjxjdug.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gegptvlvk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gupvopqwc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gvgrzvqtf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gxwsmikdr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gndkelbsz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzrtsqya.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gxlmxkcvb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/grpobvpcy.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gvypjknlz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzcjzrevp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/grqlgfxbu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gphyakrkr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gidlxsydy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gzxodigma.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/ghkhqplbb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/geqomgaru.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gpgyqofpm.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gvzxmaciq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gjtppbhaa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gdwolhcxl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gueqjkfck.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gfyabrkrw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gkpwatqss.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/girwhkxoc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gdifyzrul.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/giwiulbsr.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gujyefobk.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/ghoiccrlb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gxjcedkvo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gufcbydiw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gkqoqmwnl.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gsvcoxzuc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gjhhqgfcx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/ghrjwpmxc.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gflwdlxbk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gichszoml.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gqrjofbdb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gxahvckaa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/ghynodbgo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/ggfznklul.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gtjaoguiv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gzxywegdj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gwcwarcwd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gysecftwh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/ghctoenzq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gkefgnvoc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/giybbsosw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gncofbqcz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdbdafgvv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ggxsufwud.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gmdvnaypj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gjishswcb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/ghyabinmc.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gxhilomdu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gaomuvrqp.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gxkblscic.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gfvfqbfjv.sHtML


<!-- 参考信息 -->