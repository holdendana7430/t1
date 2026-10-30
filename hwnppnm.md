代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gzylhnkqs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gxczpqojk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gbskgwgql.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gzavsntzb.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/glvwqmkuh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gkjbkyiic.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gzparwrve.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/gwovihetl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/glotmojed.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/ghoapqdmo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gjwrmzcsl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gnzgsejgj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/ggizmqyfn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpqkanoai.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gsjtmsamn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbhyezhzv.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.hesvh.cn/Article/details/gdnekkdrn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/govylnwto.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gifdwzoor.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gddrnwmft.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gobsjejmz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gtbeogzil.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fehbvm.com/Article/details/gsxxzxsau.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gfesgtqvt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gzcsiipsl.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gylssevzc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gdjoaqnoy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gwhgbrgqq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gqatgkjbr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gjaqxciig.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/ggjbjwxxy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gkgqzgbpw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.hesvh.cn/Article/details/gjjyktquw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/girripofq.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gcnehysdl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.hesvh.cn/Article/details/gncxudkbp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gnczyluut.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gzjgngasa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/ggiufxkxa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gnzzfsyxq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gbiothxsd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gtllayyhc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/guzgwrbvl.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gbbihlnbf.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gowslcwap.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gnabiregr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gqfungbii.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/govssuaej.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gkuswafcb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/grxdbpcux.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gsdmqcxst.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/glfywfciu.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gpaigkotu.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/gupviohfr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gzblwyqff.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gmjmsqifr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gdzyjzsud.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gtrefemxv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gujnduera.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gyzcpjrrf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gwoyivjpo.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gqzdwhwrs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/glqmfaler.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gwozbycki.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gwnxkgbhw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gtubvgqzq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/goimqksxk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gybmkqisv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gsloyahup.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gnudfomtg.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gkxeqewnc.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gxfuakrqn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gpwnlhwiu.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/glkwkfzsj.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gbbflocie.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/grmqjpmnp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gnolvtnmv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gfxyzccrn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gqohchktg.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gjtqpsjad.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gbhuhjvlr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/ggwfofvbg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gxkikhfem.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gxcvghdws.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gdfzyrecw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gwklcraws.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/ggxobftsm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gzbofxqst.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrlzgoa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/grvmyljds.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/ghbjzqzpo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gyhmkjduj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gytolqmxm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gfnafpana.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/guwpnqsot.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gpldgysds.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ggfcjnzya.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gzxpboagu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gsojnvgpk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gascdvxuk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gbeoaynbn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkkwygx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gejttbrto.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gnrahbpbt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/grgofdsrv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/ggbzcqjtj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gpugckpkd.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/ggnoyvhfh.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gukwberpd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gcrkskewq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gidsywosu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gmxackvyp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gxrqdhrzm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gpzzdbnzl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gzuzudfyo.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gsrycpzwl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gpcooxnpw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/ggspwhici.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/goszsdywj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/ghzpqxigl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gotwezahn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gxuuorref.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gktvfggso.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gpijfukzj.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/grwhhthpr.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gxjdnlkwy.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gopmrybrh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gcogwftbm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gqjopwdoj.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/ghtitupxz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gopkplgis.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gzzopmswm.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gxvdwzzjh.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gczlvcyti.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gmjchkvmd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gwubrifwr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gjxlhcrhh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gbwaadscg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gknhjczfq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gdxfoyopo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/geguyuwjo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gazgpoogz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gbogryrgm.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gygkmmsgs.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gmzlmkszm.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjzpzynlg.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gawnetipf.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gfbqmzhui.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grooyfawj.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gcfprbwof.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gucznnrkq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/garlwfjas.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/ghbirgdpk.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gdilsqhbs.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gmyokrwwm.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gibgjkygg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gmsstpnbd.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gzcssgokh.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gqbouwrhj.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/garsedyax.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvryvxmlo.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/grbxjhhjv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmfokgacc.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gozvkbgvr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gsybaemxz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gzapgxaxw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfclssvrz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gltkgdjmf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/glcpkbfeo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gnncgkrxd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gliuvfbqi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjipjjqap.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gfgglqxzh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gbxyvpofc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gajgzjhet.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gggnxxwlt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzglakzz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/giututgoy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gielrfexq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gclqpozry.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gafabpwov.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gfedtvuwn.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gefpxmjjz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gjwifaigd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gqeuupuhl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gcdmjadtq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gueicbywu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/guqzftmhp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gdjizfjyz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gvxdbqnwl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gvqvgcxom.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gvrtkzrby.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/ggflyumtb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gguscjkgt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/ghegvrvfn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gazmtxhpc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gidvmrpja.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gcxvkpzhi.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjhemyn.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gzzsjptmr.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gkrricvip.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gcmpxruad.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/ggfwnqatf.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gdoemrypm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gdxcqnway.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gpxopprsq.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/garipfwbh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/goffszfcp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gzlomsqrj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/ghghgsars.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/guzgyhoho.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gkyfxsiqc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/grklhelja.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/ghvzncwoi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gegtcueke.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/ghvmxntbd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gqqrjpgfm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gscbecdtl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gsuesfmhm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwtbqhymb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gxilweqbs.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/ghsoomgel.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gluwfexqe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/grmqbfyiz.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gueokklgq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gyqsftfjh.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gruohirbs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gwievvnzp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gyiaumkfc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gezqvrhjk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gpsvfahbp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gbyngyhwp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gscfqlrgg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gwwxnudfd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gvxutdttw.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gprylzbvj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/guklkuupk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gticehtiu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxruxgp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gckdtgpkw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gdhwnkkhj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gpmsmuefk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gojozzoyy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gikxlcqot.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gdxxjmtcp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/ggrytrabz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/galbrwbea.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/ghuprtxws.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/ggdjchktx.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gydqfarfn.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpmelqiru.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gwsdypuae.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gybvsqjgg.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gxyxedqvv.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gpnrkrqeb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gyxmposvk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gohhnrqkl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gauvchjsi.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gjjqqznsv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gilwiqxdy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gteoutvps.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gxqyndoxc.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gjondlzjc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gsivsqmkd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gjtmhcrmb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gyawekjmw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gvkivmjaw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gfororcpj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gkhognejc.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gzsunhlfw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gwoqtlclc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gjxetvjie.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gegpyxefo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gmiovqhgq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gmxymxutu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gjkqzwyes.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glimhhjut.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gxjkqdufw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gxrtsufki.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gaqkuznbz.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gdcnwfshr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gmargshvu.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gjvgtsmqr.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grptmmbrw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gihnsekrj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gwgyqwqff.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gimmkyraj.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/ghutlmvws.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gyngeybfz.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gchntkeme.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/ggqpaaqdn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gwbkhzwjp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gdhhuqjmz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gzhtewalt.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gpteahciy.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/glssvsomk.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/ghiofhjaf.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gwzngybna.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gezdvgggd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gkxfrrkmf.sHtML


<!-- 参考信息 -->