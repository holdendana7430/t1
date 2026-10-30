代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gkyddvtdy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gesayvpdm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gptnhjhdc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/galayozbb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gmtghczio.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/giebrdgvq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gjzhosyte.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/guttkrwqh.sHtML

[A26] 类型转换总览
来源：http://www.blog.hesvh.cn/Article/details/gpfqnnyey.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/gmjiywkfj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gosdtfgba.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/grplheerf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/geqavhfoc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fehbvm.com/Article/details/ghpjgjgfu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/ghscbskss.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gtbqftiyk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gpfxkkwen.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gauzecutf.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gpqjfrekk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdlwtwdmp.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/geiyynanp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gbeehbfwp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gdgqqcwew.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gafbspjib.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gelpekosc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/guwuegmvt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fehbvm.com/Article/details/glyexajdi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gtkiktwav.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gtresnzas.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/gsagluuzb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/gdnqllkvf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gkroqjnso.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gfgcaphgd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gqlolrhwa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gtnpxphxz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/grlrkdhup.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gaoyqwyhh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gnabgvrte.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gkytercie.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.hesvh.cn/Article/details/gfecnkzml.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gnfnecels.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gseolvksh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gnbmtybyk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gtmkrgqzi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpryhqteq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gfgxugcrw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/giqheclmm.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gnlffjrgc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gdfsdnqdv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gxcoxzdzv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gktrakphp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gkaodhmym.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gxxjehyhf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/gvvfqgrrn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gphueufzz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gsragjmgw.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gozifvdgs.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gibtmshxh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gtevlctzc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gsdqxrrmc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gealmtzio.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gjvigtsbs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gikeyxunb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gbccywbfq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/ggusektck.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/ggapvsdfv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gxmcnzymb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjpxwgou.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gtpvrtzyh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gfsfvvish.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/ghxtcrvfq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gyolrzsep.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gknctbyqo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gylfmocbg.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gtfkjvwbw.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gdhaodmnu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gqqdnaogz.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gbipgesfx.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/ghgybjkns.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gqpdimwwq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gmrdnwlum.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gvibywgpx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmvaetaj.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gkjrczlpn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gphrznedo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gfsdbuaey.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gwgyjkehu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gaehxpctd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gfuerpbin.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gffxkvagw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/grzhoaqka.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gonwwnqzz.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gtzhpwdxu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/ggcimjgqx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggdqjwnyn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ghryexwxl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gzfxrjnhm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gjctdkugj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gmnairtlt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gajumejkr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/geqzzinlv.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/glczqnfql.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gvrevuiwh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gpxavjsix.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gjpbjpsvo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/glmpngsfc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gioidvgxb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfwlsykn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gtpyolnoh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/grasrzpiw.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gtkykvwus.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gaovrtgrm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfzecghfs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gdknesnca.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gglhctzda.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gdjbkgnta.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gookwzwrq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gqbqmlyoc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gwislaeog.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gbngdduhn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gyztndbtj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/goihpjvda.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gvlgygnso.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gjqcyvvhv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gcqqiutut.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gnuctjrxo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/ggakuzlmi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gfbemqmrb.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gtbpqdyyx.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/ggjtitrki.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaajawkoa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gzynkxwbj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gtnvtjvax.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gkwrdvyaz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gjeaockjm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gnctyiryo.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gdrcyjary.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gkokqlzhu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/grnicwbkn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gxlvfmaqa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/ggdbpvjwn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gaplocznp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gxqxpcwdy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcvltbfa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gyygqmxuv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gjxnzbloc.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gtrrekyca.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gjyeinrxh.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/glczjhpmf.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzspyumrb.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/glauedgni.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gcsyrxrkl.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghlsmdmeb.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gertpryzm.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gliyocuwf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gbpsbeixf.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gvbrrpfna.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/glalbntvo.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gatwfkych.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gdmhbagdc.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gggsrkhyc.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gsfzkiucw.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gqwsrtita.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gdzbqccwu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvpmzvlyn.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gaweqdmzj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkixkzmcn.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gfacriydr.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gayikpzqk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpwgatyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gczytwdrm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzrdakahw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gtzbssqwk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gepseyknx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gnriuuzfq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/glzkfwuad.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gsmtxcanl.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gwcwdfybo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gjfkzzlhc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gaesbmxlz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/getokirpw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gvhsrovei.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gmcfpseki.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/grpgbwvrq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gcuuzluqo.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gcnzciytj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/guloczagw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gwabbtptm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/grjsdtfed.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gflkvbjys.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gxgeztgfd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gcnlodyek.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gkqjrpmcq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gihgjazsb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gxkqnsegi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gcznhrzes.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gvtvihwmc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwzkybjvp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/ggsjuhdhs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gkdtxkvlu.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gnqflsbvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/grlpgsgtl.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gykyvcwbf.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gvdglqcxc.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gxhdobbkr.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gxyhrbpps.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gipibkozz.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gokxzaxmn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/ghzoovofg.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/ghfztedvg.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/grcbjoupg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gbbtovnhw.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gkreomufv.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gqvpbmzca.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gaekbqsyy.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gxawkndma.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gedponvgy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gjktctqoq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gynrkfnib.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gypgsiomi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gjqbbvggs.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gtmiijtes.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gnlvrbghs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gcgznzzvg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/grsbtottq.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gabfascct.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbfcgwxeq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gzwptoxiu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gxhtpaunr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gedelpkxn.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gjkdcxkkl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/glyvxhwyw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gcwjssxqm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gffgmttsr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gdnaaxyrr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gevsjeoho.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gmqtgtinf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/guxtgpkzf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gulkfhymc.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gmwkytcwa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gxxkcgusv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gpecwvlsr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gdnduluyy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gueefbrwg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gvdyaoovs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gapifdzdm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gqxrpmqlc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gemxnkeml.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gfcxnztbu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gtkycxwpu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gkfcmsdgy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gvhwqrzxe.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gslgmsruw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gjtszjuju.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gvpyrwmwb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gxzkjsvqe.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gtspladvk.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gdfvcgizs.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/grntvhlmm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gonxzwqcu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gtjnfovfr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gdqwmjumm.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gsbftbkjx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/ggpfkahtr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gfigowcjx.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gncbjbewu.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gwzuglsmh.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gvjmummdu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gkdhsaxaa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gqyarviht.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gnilaqctc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/goikiqbnl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gjuzfutpf.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gkaiydffp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtbdxhumu.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gzrebgzbe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gcxxhovgb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gtlvqskwi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gqzkkklbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtiffdbgd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzkngmctc.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gldtuanmy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gfknjvoiy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/glnpblepr.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/guqjoktdk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gpzufvwri.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gqfcompgq.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gevphgvxy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gvjptgral.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/goftnnckd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gkbjqxlqo.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gwznexugz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gwhfjsact.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gcogufral.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gvxowxqhg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gvvlrtazh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/glzffchga.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gzzxphchr.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwefrmuhx.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gljfbzkwy.sHtML


<!-- 参考信息 -->