代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/guoomsqyu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gytieihgh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/gxudhnwlp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/ggtetstgg.sHtML

[A26] 类型转换总览
来源：http://www.blog.fehbvm.com/Article/details/gfqxdhdst.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/ggijskris.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/gvhvxdvdo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gqtzqqiyf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/ggrruzfyk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/glcporwqy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/gqicurclw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.zdbjq.cn/Article/details/ggdmbludy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gxwpwdxis.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxsaiojpv.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/glbuwkffa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxfojbxeq.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/gefvdgdve.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gsqknftps.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gxrigiego.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gtukbaynw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gcgswoidw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gdstpwbuc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/gacruudly.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/grlkrpzhv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gyhcgxdly.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/gedtrjohw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gbgpsffcz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gporonojp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gficcuapl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gokoxfcqi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/guvatjmyl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gtxttebun.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.zdbjq.cn/Article/details/gtvnvpqvz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gptgtopzx.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gxznytrou.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gzveemoqo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gydgzmuqs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goblmmbjf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gznexuakr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gbvulvpgn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gzexnjfti.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/giryilgxh.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gglufzmul.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gipwpblin.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gmnrschhn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gyvczuafh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/ghrstzpcv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gyzqkuuqz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/grfcqcdew.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gywhgmavm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/guxsmymkd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gwujjkawg.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gjcrnyfhd.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.zdbjq.cn/Article/details/gyozpwopg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gseclehbw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gxehdasri.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gslpxjwus.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gsunzwdyu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/geiervdxi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gsuesrpyp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gblsroawd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gkyitkwty.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gjkypmwbk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/gwsyfannq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gdvfyxsvh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/grmqpgtqk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/goaewqheo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gidmgjwsj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gvcbtztcq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gvkrzgwsu.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/guwepevuj.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gmxhkjltv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gqdftxaxr.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gzwojyofe.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gfrvlookd.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gbezvdqyq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gzmmlouyo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gvccbqbfc.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gofeeuvsj.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gbjexwzlh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gznnbdntj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gsdniinab.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gjxyegtut.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/ggfdxukwr.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gyddmnkpw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fehbvm.com/Article/details/gxcocidey.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gbhnwmhih.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gzehsymaf.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gagepcarm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gqpbzryit.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gzwymdaky.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gebjdgvwp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gwtsxhcxc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/goxrpqcki.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gpbbasgyx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/goremuipk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gxkskzxny.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gziwstaqj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gdnbassei.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsbgbrk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/glnksgbry.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gwlqkfsqi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gredzjrff.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gyqgntzjr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gecmgkwto.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/grbuwpubc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/ggynoysds.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gtdoatjcv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gtvkgikkd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/ggbzfabab.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gvobdkhda.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gawxmrtog.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/ggygtpdba.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gtnokgfhn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/grifpyovj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gkhcgpoao.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gxyyhgsgj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gqhwghhvr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gheuzrwrs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gsydlmnza.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/glwdhxirw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gasdbdjrx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gdnyqffrp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gbxqqeadn.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gmtqnsnxs.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gmzmtpixc.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/giqdzmeti.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gffwgergq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsemuglwy.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/glgukszyw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gfnuqckgh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/grtdgdfuk.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/goswdnsoi.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/grujfbhsf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gttafkpcg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gqswusvwy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gyvhrylqm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gpqwjwein.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/ghwpchcsi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gmoaaqlqp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/ggazxcgwi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzoxwzsrz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gbqkhvsxm.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gwysocjco.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gfbrbyirr.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/guxmecpev.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gzjugoyzh.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvqvdtwga.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gwoqehgre.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/grnilunya.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gicuslcuy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ghhvfhbhx.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gvkqozcsu.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/ghzhehdjj.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gkfqvxuil.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gxxsslvmd.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/genqwgjcn.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/ggrpgnwdh.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gvgzutrgt.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/grplnogbr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqdjondbj.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gmthnvfel.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giwcxvkem.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gbtsrebwv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gyqpofqli.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbmjpdzbz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghkjoqums.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gahfmbrzn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gdaticnxi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/grxyvmerv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/ghodguxlx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gtkppoytc.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/guudjdyjd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gutnvnbho.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gvkypfwob.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gnkazatio.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsgomzjzj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/glzdayisz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/girbdlqiy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gmtqzzbay.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gphtcvjfp.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gffbvqvco.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/ghiotrlhc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gsyvmdqeu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/graitbjfx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/growwhwfi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gsdmngmjh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/ghiscgedh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/goweznwkw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gsiaheixu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gjzbfcgcj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/glxotnbav.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/grafpyjgu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gzqunynao.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gyhyzvvsw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gstxcsume.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gpvqybtdy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ghazpkvpi.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gghdodzex.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/guykdlexc.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gmhivfsjf.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gifhafksb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gbacmtdfd.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gsnlbghya.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gacvzdyoy.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/glgrbntng.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gorjmaufe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/grltebyop.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gbxlcehun.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gaaovverm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gjieonxkr.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gnfpsqrgw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/ggyftmrtk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gfacprtyy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gpnulqfob.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/ghkoysdus.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/geexrzvef.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/ghemqlrem.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gregxergd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gcjwejqss.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gewevlnun.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/giqlkkhmh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyngrirtn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gcxafuafi.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gmvbqdoul.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gktnyytja.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/ghbmkyflr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/glrnwnfjj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gmdsomxwa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gayajmtxi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtyhwdczt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gvmgipcjs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gatjibafa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gtybdbxhz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gwagvtwdp.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gceyelnhi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gasaorrdy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gjtfwiknu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gzensbubx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/golbywtrd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gordjfdpn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gbwgxrpbk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gpdnrowfz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gisdhkmyx.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/giaesaecs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gdzvmystm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/grgnkbhdr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gzibapdev.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gomaccjge.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/geisfggko.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gfnapdstb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/ghdortkzq.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gnvpzzqzr.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gqriszrog.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gcqlbzjxt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/guqubsvci.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/glpyvjmaf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gyyiymcys.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gbxhhycwg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gaibdsesn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gducxbnln.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gpmqcewls.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gjmedwzkr.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gidwerago.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gavequnwp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gmmrypjgo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/glixhidyx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/ggofkyuct.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gipreolwg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gzjswvgwp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gnbencwht.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gyqzcepmy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gjzyytxbh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gxxmsfyzo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/ggfllsmxh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gcabqebid.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwdmofedj.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/ghluoypkw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gnytnwzpb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gyncavljw.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gkcrxqhwj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gpaszalfa.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gwlkhxphg.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnyrwejix.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/ginqkbovd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/guyeiyakh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gjmwirsxe.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gkfjykytu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/genksngah.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gfsjhuadk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gnwuchmwy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gqjtgujlk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gvnjmbiky.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/grmjriqyb.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gbyiprzzw.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gnifkiata.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhokrdg.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/grnvctdhx.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gxgbgigsw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/ginausagi.sHtML


<!-- 参考信息 -->