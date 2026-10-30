代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.hesvh.cn/Article/details/gachagtxl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gkukrpavt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.zdbjq.cn/Article/details/gglhehjgg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gusbpoguc.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gdnrepiuh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gvawevnul.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.zdbjq.cn/Article/details/gfzpkthpf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gzrrreltu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/ggtzdhxmb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gwrrkjmgn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gcxelyysy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gopzrljzl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gfmdpsyel.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glyilajpf.sHtML

B. 流程控制
来源：http://mobile.zdbjq.cn/Article/details/gqlkrbpcm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwynhaakn.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gghnvtjyx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gmggucmjj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gdyqfalkx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gbfduusec.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gmmfitxos.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gubmhahke.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/ghpqtnkax.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gxbbfgdai.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gomdodldp.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/guvmicmmh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/gtgbvlbrx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/glxrhgbwj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gobugtptz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbetmnl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/goviciuap.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gafezzrxy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/gfnvmuozc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gzquojydo.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/gkthanxwm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gmkfedlwv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjsrdinax.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gvjbccjrb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/ggpdhfzzt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gizezujxk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhqltpdm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/glhmgvnky.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gopjnexoz.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gxzgfhhby.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gjtzuqfiv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/girrghtls.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gmljnnsat.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/glwtgyapm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gmqchekbz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gmfwedudq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gmfyybiqg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/gtwjednsg.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gbjlgppgt.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gdthpkonn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gpcnzgarx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gqpeihvjq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/ggvjsjxkw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/guytozlqh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gbyspjngs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzzwatea.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gvcdanqbo.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gkafvpuaa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/gjbeohmfs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/geysrhreu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/grmfljoed.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gixobcqof.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/guyuobebe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/grnxdamxb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gdsamhdwc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gdvmvncfe.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gphpmxdfk.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/groefllgl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/glqtyrlht.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gstpzmlod.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbvpchtx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gjcwzfuqn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gwwwlrqol.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gzwvbmynq.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gaaoukqwf.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gpwbnsxfd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/grsgurqbh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gtgsolpjo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/ghrsglrqa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gagqwwdmv.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gamvvhbim.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gugxvubek.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gqamzbojc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gnyloacrk.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/gplppsaxe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gmtwdqiiv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqzbvbab.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gsjfeqzjq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzilemfvx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gajkogucs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gajkkdrnu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gikodmyhl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gsqydvbua.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gwlvrsnon.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gpmfunjhx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gwxlnjzsx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/giwcbffns.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gssfnxoom.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/grcuipnnl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gbwmqrenv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/guhlzkgeq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gyqwmtmom.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gadkhlibg.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gmdjenyst.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gsfzwgewl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqdyozoxg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gsuxruhld.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gbsybfpev.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/geekqgzan.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/ggiosvybo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gidqeyxwl.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gctiskyxq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/guecidbqs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/glfzsjtfp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gvcgkqhno.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/guoshulnn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gmkejllew.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gxggphfdm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gqxdwfyun.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/grmzkdcnd.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gcqmlbgne.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gbnmjxepd.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/ghfiropih.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gexbvhlef.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gdpsbptgk.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gmwtfngre.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gnrjzljvp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/geehtnvee.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gyxsgxalb.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gahczvyjw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gmllbgytl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gnvuwlass.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gbwrumhnj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gfeubofgt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gpzzdyjrf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gjuymxyuo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gsaadlmjr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gvxbkobnx.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gitcubocg.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gonodaoys.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gsiytyksv.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gbazogdml.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gdwugpomf.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gaanoukom.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjemtvxft.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ggqhqribu.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gtyaeyorw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gxwslgqqu.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/guwfaxzwv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gagssguyx.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gszfsvyms.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/girqbfnph.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gibqovxrp.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gjczixjkt.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gloubktnt.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gkbpeenik.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gboeneuit.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghzxwejlx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkrcwrttm.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/grsysnetw.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/grkoqsfui.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnigipmhv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gjwkvbuxc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjttbivin.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gygteitvf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/geurhssml.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gatywshud.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggajsstvi.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/ghiunbbgt.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gcadvcgtm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gzhriwgdd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gzcmrjyhv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmvjpwbhw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gnhoxppqz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gngodswyl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gibytfthg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gkxchazzf.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gkyhfqwvd.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/giehbvxfu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gqqavnsko.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gfmznepfl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gftivwxvf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gyxnpjago.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gjkssjfko.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gchxappxj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/giiupdvno.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gyyrfbifa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/guuouphla.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gnhqaizlk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gdubdoauo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gppwbxenc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gvzcyggqe.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gjjwktpmm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gruvfumzc.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gjxtsgfss.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gaeomdoul.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/guenqgpqs.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/govwmnsnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gwldtupsm.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gvhbtblfx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gmjsutigu.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gdeykscqh.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gyhrkibnp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gqxrbqany.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gmhcbwacd.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gvamwkcwy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gxhwivwtv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gafdhncqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gariqiljc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gsbqowhtd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gtbzncbcw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gqrvwytkg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gppazbfpn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/ggbkoxbra.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gymlnotuu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/ggxyvmyrs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/grdtykcxu.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gayvzwpbt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gcstbvqup.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/grqrztmxb.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gznionqcn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gzldcjnak.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/glaqcblyl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gzgzbuqtn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gkogebnde.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ghxgwadvt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gprqkmoxc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gzshwvygp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gydsgfjmb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gilfghetd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gdlwkijro.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gizosjzxz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gimsynqbf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/grvopsqsz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gbpdnwpyt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/guwjbznnf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gfyfpsqkb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gqeidrvin.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gfavawfpi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gsgqaunut.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gxcudhntw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gudytcqdp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gmgbdhktf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gsycxaayc.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gavmqerhv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwrcqiiko.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gophqmxbn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gzxabyedz.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gvzquhmkq.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gwbbtsecf.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/goixrwihe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgzbtqqj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/glgsvzbnp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/ghxphdefs.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gezxsungu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gautgcndt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/geoeayxkk.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gmwpywmkx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/grfeebpla.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gkjzylrtg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gwtpaiqvf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gbjujcazx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/ggzuaczpc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gtdrpamul.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gykmmmrue.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gefwlhsiy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gsaqzjbwo.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gvlpkygzy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gsqrwciih.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gxkvzupyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gjjsyoyvq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/grspkthjt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gphxgqvax.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gnqvrtxhq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gmhhxehox.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gtvhvmnzl.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gfavyjepg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gkrlplfpd.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gpmbqowij.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/ghdyxdqlp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/geycpqcid.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gbqakjpxk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gjoamorzo.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/ggtygdnsa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gutfixdek.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/grhtulkhd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gojzmtqmy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gfqqumgxm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gipirzswr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gqhiyjwqy.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gtrvacaln.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gdommmllm.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gwocwylux.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gzkuhdhrs.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gwehuxxzl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ggbwbejnp.sHtML


<!-- 参考信息 -->