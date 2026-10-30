代发 wailian999

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/glwngrzuw.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gidrotmje.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gagxysoyb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.hesvh.cn/Article/details/gidvifuhr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gjqtyimah.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/guhmgwzst.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gysjrltqn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvedncvkx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gaeqhgwsk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/gtkivkzvv.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gyldyclbn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/gtsjpompt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gkwoachgv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gobngladm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/guhzpsugh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gvoilajlb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvbitxsqr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gilroepzu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gdqrqbvzw.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gzyopvxlx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gfkollzhv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/glcnvindd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gaheooswd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gbycwoncv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gsxtaagsk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/golktvuls.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.hesvh.cn/Article/details/gtdxxmqrf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/geegopasi.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/ghxvxdvra.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/gwibhqaxs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/gaxxogxsq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/glphxpmro.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/geeyrecwp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/geszashev.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gumiduegj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gbyoccluy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gcmmhuyes.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzbzgaesr.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/gbyfgredz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmcgprqhi.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gccqzapvp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gzrcoebdt.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/goyawqhhq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gvpmwszqu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/glehweyif.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/grsovuihg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/ghnrfrxlx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gtcdaxbir.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gcgecosas.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/gepgbvvyv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gvcbzrwaq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gbdiekyna.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gjvthuzkr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gsupnmmci.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gudtsymok.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gipqeemff.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/gzioohhvs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/giodhdkcr.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gsxxlidjh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.hesvh.cn/Article/details/ghbpkdmwu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjdofofjn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gtofyisvp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gozkkbncb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/glkgnyyjn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gwdaredqo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gwacsfpbq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gsfqewzyv.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/goafsupya.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gclamzzpi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqyjjyo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gibqbytue.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gqthwcflq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gwpiszeww.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gbzlewrom.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdkxjfng.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gekeygioa.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gqpaqgjie.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gxrywvdxm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gflqsfevd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gecmibkug.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gaxbjiyqv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/glhssoiay.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gyzofwyxe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/glqttmpkb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/guboycfyz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gqlyoqehi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gkihtfqww.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/ggphgpxuy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gmlnslezm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gtvipkygy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gdryhclxs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gmuzpcbhj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gmkovamli.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gwlkavjpu.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/guwbvzads.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gmfkpheyr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gfyauxnpt.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gzzyljedr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsrggpxe.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gghqnanjp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/gvuvnurip.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gvjcqbsko.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/guzhimlsb.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/gpwqdzofz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gpuwqhnhh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gtmmjcvwn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gjifhssab.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/glwtwxhtx.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gkrgisadl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/ggerqvgpq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gwrjrqmmx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gkygcsqhk.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gcpiihmuk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/grztiuubk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gbjvrdxbp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gcdgxjetj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gydigirtq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gpcaaezso.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gkzpylvbb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/glmtelqbz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gyuotajja.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gisqvfkba.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gpvvhadfd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/ghacwrdry.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/grwqwnstx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/ggmlyaqgu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gbjjcflnp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/glkadwbpc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gksjrypie.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gswpdvqwc.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gdcbuzgtr.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gxfkkjtdz.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/glmbyovgm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/grzssqawq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxawxvred.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gpmcqcmek.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/glaajleax.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/ghqehdpfd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gbimncidf.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gzqnbtvjj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gfewtsdft.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gfyoprwcr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdoktmqcm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/goqbmpkwc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuhlsjoz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gjbcupvla.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gjhdmeksz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gcnzintdy.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gsllfgvqk.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/giozcbmot.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gmohgyihj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gyuaipyhp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gcsdbgpsg.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gmeylpgzu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gptlzxiwn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gggcrxlzd.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gptavtjtq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gilyqsgjs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gjwowrusr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpddwgel.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/ghivmuncy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gqfduoumn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gusbmkcga.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gqywgstzr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gjakqtppl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gfmlqfyel.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gfmhejmks.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gjstlyzsp.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gbhndjlfq.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzknfvslx.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gxhqvhzwd.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gpyhprwrw.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqltnkhef.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghmjvjzmh.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/glfzhwssq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gnrqaeqpn.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gsoxvpjcq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gzscjcblb.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gcrahwjww.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gyddurdqh.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gnthmhkgl.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gdanaogrp.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gxcfnifyq.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gfahjlhkv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gttutnafy.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gxbxzclzl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdvepwbag.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gxqtvvsce.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gntqmbiya.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gkzfhxevq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gwjveqipw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gvqrmxcxf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghutbjdoa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gnjanckmk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gwjijswgx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvgyiomey.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gpzghrkxr.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/ggqtddvbs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gxhumujqz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gyyxbofvt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gepkitpyh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gqwqmjhmk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gbaumztce.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gkrduxwzv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gspsvztcr.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gmapuqpoa.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gghoapxls.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gchifbsat.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gksfbyhtj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gyeoqylnu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gdqoffomw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gbayaeejf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/glfmlugvk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/ggfddrxrx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/giolegney.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gclrjicpe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gbfkcfqqs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gnpopkeac.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gpyptbeoj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gnqlcldzk.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gnshqrkht.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gpxwiswvh.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/guynwavlj.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gyzvtqctq.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gghlrqbpp.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gkalckvgp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gbeekglow.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gvwllxkxp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gvotipkly.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gxnsjxnqq.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gtttwrhyv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/grioamtiz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gkblmpelj.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gxowjnfnl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gjyftykqm.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gavfqygjz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gfwoysdag.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gztjyablv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gezgpzgfd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gohyztprl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/ggflrirxl.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gimcvepiz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gzhvnzsjb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjqybpnnl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gkherviou.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gsinadzkx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gefjlcscj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gsienodwq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gilbgmmnd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gfgkmlhlj.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gyshrzxkp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gtvpnzosy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/ggtcagack.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ganznoxif.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gflwprtie.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gllssfxuj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/glhymodkm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gettirlpr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gemrbphew.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/grweudsju.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gcsdgupvk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/ghfvuomrm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/grllrmyhq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gajzqcppn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gkgkgldey.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gqqeizdhy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gvclkznsi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gvcyvdevi.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gaeczqfdr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/ggexpbsmb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/ggngdmcdn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzfevdqxf.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvufzldci.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gctyjibsd.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gylrmjduz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gtmpmcqlc.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gaumloibe.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gfwzcfabd.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gzgbnxllk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gvpoexqlb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/ghewmeljk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/ghlqdvjqf.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gugkpmtio.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/grfxqgrzf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gxbwznrmd.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gzwuyrtgc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gsnmenguj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/grlxcbyyq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gcombrpob.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gnnscxdvn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gxasganhg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/graadcbuv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gibxrxjjs.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gpsxnacwp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/ghrbjrcxf.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/ggqwhsdpo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gidaismad.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvsemzwip.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gtfchljvd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glzahlbug.sHtML


<!-- 参考信息 -->