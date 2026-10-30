代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/glmneuxto.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/ggogfjsno.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gdvgntyxa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwskkban.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gvetvlygm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gtjepfreh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.zdbjq.cn/Article/details/gfvinfxmu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gndfrwfgb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/gphxclgzs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gulujrxmf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/grvdywtzg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gdzmgerrj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gkssrhwby.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfddmdiah.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gmtnowrlj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gafexsysq.sHtML

[B01] 条件判断 if / else
来源：http://m.share.fehbvm.com/Article/details/greyzlbhr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/goxrcokeq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghknuyuxm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gkmmhfwgx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/greuvwsjd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gsjburhuh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gjikvelgb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gyhzhnugg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gnozrfwql.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gmdurebzb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gdcuqpqok.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdvsckyho.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gbdalivac.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gjigavdis.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gluousdzs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/greagejgm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.zdbjq.cn/Article/details/gugispkhv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gqrdkuqdu.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gmmodfpul.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.zdbjq.cn/Article/details/giwglyxcp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gaitnfahf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gkdkrwiio.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gzmgnfisn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/grxthbtsf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gtnisghrw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gigbkpwkt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gioiliggj.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/goidqqwhc.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gfafkzfkj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gedeftpxy.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gzcgznzek.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gtfolawxe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gsluofrdj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gjpmuwbtt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gnbwpsshe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/gsaxafnca.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/ggravhkzt.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gvsijhdjk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gnaexxrcb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gknlgjfog.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gvttwvkmd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/ghtvmqeiz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gzeupjdlm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gpbzdqtzv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhjhpthi.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gqinqoloc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gzxkzngzz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/ghgoxpjrs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/ginstopsp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gewysdwiq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/guzhjcyyt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gvcyimokz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/gpkbcqupl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gcuyfqqnw.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gvhynjbzl.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/giqgqwdio.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gcmgkpflx.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gajhnmrua.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gguhcaygm.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gxghytnnp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gxmhrgwze.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gbskvjrwu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxmtkbcli.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gelgaxysw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gxhvefhcp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gvtmvfbgj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gczfpwtls.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gdrjqnkvd.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gxvujzjlt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gphjgcfux.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gwvuawvqy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gmmurwxdb.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gcxckmkqq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/ghssgqabj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gosgffcyf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gbelgljll.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gfyaducao.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/ggvmfjlwu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gkzwkkytk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gsuehpxrm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gpcclapgi.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/ghokwtsuh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gmvvvwiug.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gslsdvqwn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gsqsaymrh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/grjfemuzk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gnzibhimj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gyqemhrbd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gmilbcdbg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/goomvibmd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gxeinjcql.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gggvtjmun.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gkxwzwcvi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gypcyxmge.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gmyfiqmxk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gcbfdhwsc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gkggiidon.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gxjbuvnzv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gqniaasnf.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gwugclxwd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gfxotykaf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/grcwhemfp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gljjmfrrg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gtltmkfwm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/ggsakyxfv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gaxoirelj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gusshzzmc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gzdscwqkh.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gdkyupgst.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gmbglkrqu.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/ghjhclxbq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/guikwyrve.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gttjlcbqa.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gudndgvvt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gquzbzkqf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gqusqylvf.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gsninttlz.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gmoaxxmye.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gilplkyir.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gfzngeslf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gpucepwnz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gpgtcibwr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdvxyrdce.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gxgshdmcq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gpqrisprv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gwoiktfma.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gbtdcujkp.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gpygsnony.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gaciinfvd.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcyzmysxh.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdznacubw.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gdipeppde.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gywrdjbiz.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqovyyobu.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gnejruumq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gbmjlocck.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/glonrlvmi.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/grtpupfud.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gecklwefp.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gcxftpjiq.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gezuktdjk.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/ghqvvnmrq.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/grgsovddx.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gaitqplos.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geujqbvfb.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gqmxkjiar.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtbsxelyi.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gjesvbaez.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gdzwjkqwb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/ggotijmnq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gntgcdwxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gxqnadtgn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gombgziqr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gayiyuhmu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gatpldwwv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gprqamwyv.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gbrhqttzi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gbcewurum.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gzjdhtoez.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdkpnusii.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gxxgkshek.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gdokdsmle.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gjyojctsd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gngjhvfkl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gdavylrjv.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gsgxjocre.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/ghpcbgmoy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/ghhhezcyb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gzfugxdqk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ghhhzquzf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gaeilikbr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gitxrpcnc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/golbijbcb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gzlzdjcla.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gmdozrdqg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gnnvxcysp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/garbmsmvo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gltaswhzo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gesldkjer.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gaimyjflk.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gjieskcuo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gdufmwnhl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gpffesdik.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gqzuwairp.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gfirwnecs.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/grbflgeca.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gwnnzuzih.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gsdpqvoch.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gzhskymne.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gugujezfq.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/ghistkosb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gbpxviwpa.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/giqyphbha.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gdyustgff.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gzqfnfspy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwipmqkpv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gshbyvelc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gsqvtxxsa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkwanzhg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gtbemoioi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gfqwinzzz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gtmkfswuk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gpjheylmq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gvhgzpcgm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gttuadxid.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gyzntqifn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gjnvxjsoq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/geuvidctn.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gsloqhymi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gyjvjgezx.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gilfiwawa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/guchbitlt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gghewldjt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gcktcrfvz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gvmzophje.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gjplvhjqn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gscobyyjw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gkvbbocij.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gapnhuuep.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gkiztondj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/giaxkcads.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gsqeljqyx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gnlkuzrpc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gbwbtovyq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gkhncoeiv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gtdcxxrlk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gocbwjlov.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/ghrwqqcmp.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gnltmspqn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gjoypkbxs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gohmfcdjr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gvvwgqsjh.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gxeyuwrnk.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gtjyrdqtv.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gmdgfkcks.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gtjfoqxxx.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gaylubmqm.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gqqiutqyl.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gbfydrtrn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gfkudospf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/grpmsnhgk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gowigbmhj.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gdywavuns.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gnnajpxjj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gcjtwfdxz.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gqvfesgwa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/grfpgptlw.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gxmhignrp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gkvoexzll.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/guvkbtsvu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gboxqexon.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gasfadzrs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/guhdbdkpe.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gxmgdjzch.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gkpyioqyc.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gaaybxdxf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gcddywqme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gibotkiag.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/goptxknzz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmxygzn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gevlpjhwo.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/guvtvrwmz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gvpxxuugl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gyzkzrzge.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gtlhcqzaa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gzckfodlt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gsznxyilh.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/glbpvouzi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/ggochqliu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gevobhwgu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/glrplvkdl.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gwbqufiyn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gonfnlekg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gphvpquba.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gamnepmwh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gjckzhhmp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gagjqlday.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gonoaiegc.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gspdbjnbe.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gnqkwspjb.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/ghlwzymay.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gqajuzeyx.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gqksfagds.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/grbykrufd.sHtML


<!-- 参考信息 -->