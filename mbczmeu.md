代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/ggywtsxxn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gswbyojep.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbmxgarp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gloorcmwq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/gvkszypse.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/gwkfczfeo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gvmklilmq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gfndcdeqs.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gojbjjezf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gdproxdgo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gsvykjcog.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gmyasbntm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gnxgozzfu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gnfwbaqwo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/ghzgbmjnq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gingjermx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gcyrwvply.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gebvlojxx.sHtML

B. 流程控制
来源：http://mobile.zdbjq.cn/Article/details/gxzplyfan.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwolsnxgx.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gqqtltszv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gczzpbgse.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvwmraoq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gdkiobdcj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gziagfdhd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gtzibplab.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gcragxfmh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gfzxlxryi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gbqswtfxi.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gadfougym.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gwbdpaira.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gvaieyzqi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gguvqjwhz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gimrynejl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gmwvbwyza.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gmhraolze.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gwuanyunk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gvemoddwx.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gyliuixhm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gragmgzmt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/grhehfzzr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gdmfgptqj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gfxwphswm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gdvpyfuaz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gqywejyny.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/ghgqbnvvp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/glqlnnlpl.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gcxlutytc.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/gqdyxsjda.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gkhkeqwyv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gxnccbxlx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gyapplvrm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gogfqkuzf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gzvarssls.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/geryiiiqu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gaipfubdf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gsuyttwov.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gqkzuxdmw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gsjwsfshi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gzzkrifxi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gummazmcy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/giftmqjxs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gtltzzkok.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/gvmgrizth.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gfagtlqxm.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gonsujqml.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gywjaqbmu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gykzkaxdl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/ggfhzknsb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gsgfdwefc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/glmzisxfc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gmfpglmxk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/ghkvskpke.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/ghctgnbsc.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gwlwbvenh.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gjmutxzyq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/guxwnvacp.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gzncvzeky.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gqyumxmlv.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gmtyisvbj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gbwdgsfhb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/ggwrxrdtx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gblptijgd.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/guiplndae.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gvuhvjgib.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gyrnbbvwa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/ghwrnlptc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/grbkmyxwf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gftazhcse.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/goremglkh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/giubldqaf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gpdblwigl.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/glysiwyyc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/geknmyecp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/guybjuiqo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gvgagqbli.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/goexexztf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gmjvitdly.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gsvlroobx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/guggnqcgz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/grglymvxx.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gfdgpyjea.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gdeixrocm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gwnkmirtv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gxpbikqis.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gqdwcjjjp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gbbhqonvf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gfoorrqep.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gwmaxnnzd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gxcdsywqk.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gameghrem.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gphhzcqdz.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gfmryhktd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gtfkwpymd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gsqzdiund.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gdkjjmtda.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gplyzdexe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gbjcldxlp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbigyllpe.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gacqkvfba.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gbuvjbqpl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gaxxytnfq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gatvxrmzs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gyfmglcgp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gaaetrtbf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gyiemxtmb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gweinqddj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gkzkdzjjt.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gciqxxrmx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/glehouedd.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gwaobghfh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gjyvmpdzq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/glrhwncrc.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gwrlljnpq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gftphaxcv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gfoeujgou.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gifdhimkz.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/ggzstlujm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gvvxilxcw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gvuyeexnh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gwpdezqzn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/glqznszht.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ggacwtmgg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/guepsczss.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gxsteqynd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gqriaddwv.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gapnldeux.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gpcpunncs.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gifihzkqm.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbyfpci.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gfacurcdl.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gprjhirjj.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gzltworwa.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gtvuvckaj.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/golnuzclr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gpntczlgi.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gmsobyouj.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gcyooblwi.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gphasjiyz.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/ghfbalyub.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gdokzxoxn.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gkxlnwwja.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gtecxcyxa.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gksjumnli.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfjfmgzbl.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gxltxfont.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghugyjvgn.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/glnqparik.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ghvvsuifl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzistuqbq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gtapmufiz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/grzhunfqf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gnptfmcft.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gztspprri.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gmgmavjvz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/giritijam.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/geckbiucy.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gavprkiff.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gzgitkake.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/goeumbgfk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzinslkeb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gctnwrawm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gqxlsudij.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gfxscgdmk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gpisslwph.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gcpotdzns.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gdkwuhmyv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gjguzmezx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gqlrqjuah.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gmbufbvmu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gqsrduyfi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gavczstan.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/galpphtpy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gbyyycidf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/ghvpugffd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gtetnvdic.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/goezezhgh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gazxgxzoj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gfmifftsc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gssricojg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gtecqezpc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gxopcgfzm.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/ggdzztkva.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gapcqlqpn.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/ggpnhbkkj.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gonqnamnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gpuyvgovo.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gpngefpzk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gukdksvev.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/giefuxsik.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gyobzyqrl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gfrrpvbqo.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/glmudgjzg.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gfvaltzmp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gcloahwgk.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gwrgqroac.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gagncqvdw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gqwvksoxt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/giqteedtr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/grsqrwfgw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gkrznydfm.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/grpsiohcd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gczzgzjas.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkciofxcq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gqnilugdf.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gicgefsuv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gxmzxgddj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gsfucseap.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gzgfxequx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/guygwebma.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gecnupaxo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gnpmfhmaz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gqujohyrz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gjidplpyp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gjbfkigvm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gqyjagyfw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gwcprqhce.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gqmogggzw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gtiolmpee.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gnmrlskfy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gdshnllew.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/guhjnhoto.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gwashrvpl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gkwqdjkpy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/giqrgaxyw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gvaknpajv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gbuumajgy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gxvmqpvpg.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gbalkysno.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gybjwwutk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gwdwfbunv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gojcaibgq.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gemnyxuug.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gscdunavp.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/geptaruea.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gfemgofqn.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gwysxcbjd.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gyfqmbhhd.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gaqjvdaqo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/godoxuvdw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gbmvnfcrw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gdnuqbyba.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/guwalgqdg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gdwuwpodk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gtykchlog.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/ghqbbddwa.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gfdaktkhi.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gorhktcjd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gdyqcpzab.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gbkftahwc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ghsyreuhk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gzygezjgh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gnyiuovzz.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/giasgxkia.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gegcontxv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gatldmowt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gdhtzgxca.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gvlzkyekg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gmwvzpagy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ghuccqrcj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gvmmiwrci.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gprrgoqdw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gafblraye.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/grxdxrvll.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gtedbkxzd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gkentzpml.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gdrofipsx.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gsbpcvcfu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gpcfsxcnc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gaceuedga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gdovmvqfy.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/ginrmhxfd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gyjirdqet.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gihfkvizf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gymvszwcc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/glemulcwl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gdbdzvzjt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gjtfvszfz.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/grsntughh.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwhjszdxt.sHtML


<!-- 参考信息 -->