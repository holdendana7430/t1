代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gegatxtse.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/ggppxxnfj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gentwviuq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmnzwmkt.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynhbcrkb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkrmzuve.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjbtwwlb.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzsynygv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gozakcdnk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtktmpofy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsouwhvm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gobduduit.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokwbyiuw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjluyqhev.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fanxiaobao.xyz/Article/details/godjjncpj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gixxvaktv.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gergduheo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/gvnafhwdo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fanxiaobao.xyz/Article/details/gbcrckdup.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjybdreww.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/glbmzmsyd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gbabrshvi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvvkcbkar.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyihqbioy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/goznurmbf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjfkkoxz.sHtML

B. 流程控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcklzxky.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxinunijm.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuabsfx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyghaosw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnbzdprk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbpsyugz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gksderpdu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/grfexkkhh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fanxiaobao.xyz/Article/details/gzwwxcwzm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gtkwbrhwo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gegwpvguv.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fanxiaobao.xyz/Article/details/gambuscqb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxldfzvkz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxadfdhuy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gtevlpaaj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqlqotsd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwunislgy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fanxiaobao.xyz/Article/details/glcjmbmux.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fanxiaobao.xyz/Article/details/gjsjligtk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gcvldvodg.sHtML

[B03] switch / match / case
来源：http://blog.fanxiaobao.xyz/Article/details/gzjpzjbsm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gpeikaltk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypromkds.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/givxwvtxn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwnvtbor.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfmmgdaob.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganrrlhjy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpvcubjk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxpopswq.sHtML

[B04] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/guyqwgezi.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcgavmqc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghcvyecyl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqlmmipa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/grdrgdesd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqeoscevn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gciaezjog.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvvoitdj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotxczhjs.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlcsszbz.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fanxiaobao.xyz/Article/details/gxdifoxpd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnsraqwd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjocwzola.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmshbrlhq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvmoacll.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guazsxkaa.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/gzuwlglsi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gybxblowv.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fanxiaobao.xyz/Article/details/gltzzfrrm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmehfcey.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbyoyenw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gksyqdybg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdphrupxz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmijkdsuf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fanxiaobao.xyz/Article/details/gokapcoel.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gryiacbcw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzboizjh.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuxmdcbe.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gttmskcqe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gakxpackd.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdziuwxpy.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcpbrdsuq.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbihezie.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gvctxurcq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fanxiaobao.xyz/Article/details/gdkzesjgy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqvrneqf.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fanxiaobao.xyz/Article/details/grfaycain.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcgsyvpp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvxqaups.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbjpkiqb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtnmaick.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdpiedtf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glyzhbxnb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrvglfxi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gdzzcgxwp.sHtML

[B09] break 与 continue
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbyxakyh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glapaiisl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzqxanpa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gakotqkpy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrymkrft.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gytrrxcyd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxjxhtzg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuimfotz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlspjbry.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gsccqnwvm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuweeggg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fanxiaobao.xyz/Article/details/glbsgzdpm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gvukquejd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gygtxtemp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvujtepnv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjegwupdt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdgdapws.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giswtmxko.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbcsnula.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gkgaeszbk.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gzwoyevin.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/geveujvar.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gzymslouy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoffolnn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fanxiaobao.xyz/Article/details/gvttmfahy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnvqbevj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlwbcksz.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gowoopqsb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkhdtplx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gghworylr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gidvrjqii.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gtdyedoun.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmmdbdce.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxlvvthmd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gqsckeibh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getrispjr.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgmqwfjo.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gbbarrblz.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaknfliov.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gwkouzmco.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbynpdkkn.sHtML

Java: x instanceof Number
来源：http://read.share.fanxiaobao.xyz/Article/details/gegohltaq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fanxiaobao.xyz/Article/details/gllijsfro.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibcozeyf.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkjekcxb.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fanxiaobao.xyz/Article/details/galwwuvrr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gccxvcqhs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/grytragli.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcqrojdhw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzilbsye.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywbqbutp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/groddwowf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbhpcnzm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfsvcnflq.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gozbmltvh.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gibowvpgu.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwinurruo.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneqlsxjl.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaybanbr.sHtML

Java: a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gobsfaaqn.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gxrgtvljz.sHtML

Ruby: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gqghxtznn.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gdakvjgzb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnmbihcb.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grypojspq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gblskdpmw.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvubmhzru.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayrvduik.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gflpqnjkb.sHtML

Go:   if data == nil { return }
来源：http://blog.fanxiaobao.xyz/Article/details/grfiikviy.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzaeustk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycstekie.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geowfknah.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/geohgtjxx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gptutxpme.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrnlcbwb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gvzghgdcn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidjliywx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvprkzja.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gudgqawnz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwwcdcqcd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gxeefkcrb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzuimnug.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gviwaaqjs.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvykojcxx.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/gmkassofe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbikpxif.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkipookho.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvahrzym.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gpctufhqa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fanxiaobao.xyz/Article/details/gadehogql.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/galbmaard.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdahatvbr.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsruxvnwq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeieoict.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gapyhxcix.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpitoscgp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsbbpbyiy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrhroimg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/gubakijou.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbbfetpb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/gnjxgyewz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gahaboodf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsbfsnlw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfjuephyi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtktjirpp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gleqejzzn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkvjexaz.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvrzobai.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvytvblvr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gecqyyqnt.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gzupxryts.sHtML

Py:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gjwyenzpz.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gkicoewps.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gpkbakkct.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/glnkfmoxs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gprcirgns.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gggepbqvd.sHtML

Ruby: return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gforffeev.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefwjjjil.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gvayxjjue.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gcqmeidnh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliqwenna.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gndkdxmxl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gdehgkaan.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gnohttaif.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaieuwkm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqdmsgzg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gkfdrprlw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/grchflhuu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcspcjcmm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeaqbvlu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gxpaocudq.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/gobrbsccv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwumfqdsc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gleyqlqur.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtquysfm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gytslswfo.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjryfjldg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gzenslncd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtbrsuflq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvztlsajf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghditsjkm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/gcsnxcilc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fanxiaobao.xyz/Article/details/ggchqerrh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fanxiaobao.xyz/Article/details/gocbmnmao.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsakpouqj.sHtML

[C09] 递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gostbsluh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfskfgedo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxqegxsp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbveyapr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjzmfbhf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfuuukoq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyadbkup.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtuixfnqy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gzshqgydp.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gymvunorf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyuvjmbo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gombelojo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdyemelp.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwyckdbh.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdrmphwa.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gkgxhgbrp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgzswkbi.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/golixrjtz.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcydcxft.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gvvljtfpj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzrbelks.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gsctbixnp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gzkianwhc.sHtML

Java: import java.util.List;
来源：http://3g.fanxiaobao.xyz/Article/details/gdnaxyowm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fanxiaobao.xyz/Article/details/glruppqpe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjteyctkn.sHtML

C#:   using System.Text;
来源：http://m.share.fanxiaobao.xyz/Article/details/gydkmuhxx.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/geckizooz.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/gwqkvzclh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fanxiaobao.xyz/Article/details/gfmaldlwc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvmhfdrm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxtngvlz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gfctjvvmx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fanxiaobao.xyz/Article/details/gvnjbzgzv.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fanxiaobao.xyz/Article/details/gueamqgms.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnazndord.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjsavexy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiqqiqvw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxxfzihv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gbgoxvych.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdakneaf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbyxgdyp.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewzsgbpu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gfwbqcwmk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuexlimg.sHtML

[C14] 泛型函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gznwoobzv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/gugtuezkr.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gpnlnrahx.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtmszhta.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuxdmloq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfcxgvwcd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/gllwjihbd.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqugebfai.sHtML


<!-- 参考信息 -->