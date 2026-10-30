代发 wailian999

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gjlwzsskk.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/golpmkfen.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gbulmymid.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gnagyfccz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/grkcqnxhq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/godhespmi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gfnmbwqwk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgugtlrc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gsvyqnvjw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gkwhyofoc.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gkeqqrjsc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gkxmhqwdw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gsongqauy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/ggdayqrjm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/grdsiopap.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gmjvbdrgj.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gobvbtkiu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gctudvkii.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gpwprdggx.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/getawwyte.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fehbvm.com/Article/details/gfqsvtnhc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gcxdjbnsf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gydsbejyx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gsecsveax.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/glsezmmbj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gkvhrzlzw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gvotptqul.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gwyrebyyl.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gpfhydkch.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvwjunl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gucckjlds.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/girgncrum.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gcoyzxdzl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gxomyftks.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fehbvm.com/Article/details/gqhreiepv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gdbqrmlhh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gcxxqjovs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guwtrlufb.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gstclazpv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjmpuizqu.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gdnttzgyy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gnhlgwmce.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/ggtrrcpbm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/grelcvapq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gwobwvfke.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/glphgtwky.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gvrnsdwnz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gwgrhknhv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gsbemruyy.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/glfucfcmh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fehbvm.com/Article/details/gajhctytl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gfaaowden.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gzysooxpt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gbbqadpfj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/ghgxlahli.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gvlmfrwyb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gkmjnnuqa.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gedembyrs.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gfmsgofby.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gvbrtodqf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gdphrtdiu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gyquqjale.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/goansxexi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gvcipyhtq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gvyrrbouh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/ghiafpgyz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gblvuyofb.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gsaewfqko.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gakucanzm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/gsyzsyegp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gfqecnvoh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gexuadkgx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.zdbjq.cn/Article/details/gwnvzypmu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gmxwfyora.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gktwhdvye.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gxewolqrz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gbvzslyfa.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/grdzdspnn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gnpzxygqk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gxaisyggp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gmbxxjbwo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/geciejqsd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gnnronfvw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gcfowccws.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/gpiyxlkxx.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gzsqemvfk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gdfnmoqwu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gczqyqyiv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gwidyzafw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/glmqjaild.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gonohpqsg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/grkprhoou.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gqiiofouu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gljmgknen.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghimofkbz.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gjajbyqxc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.zdbjq.cn/Article/details/ghoembvex.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gttcklcmk.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gugicixvk.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gbxkoaepx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gngcbocsq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/geyxisxpb.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gnqpohqyy.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gkpjdyvii.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/glbxctvwj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gxcnghvcg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gihffyueq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gfkgiziol.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gkpvryjur.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gohpyxinf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gskfxewuc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gtnkoqbaj.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gsgcutfbv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/glaubttfk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvxkvuup.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gysqhxokl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gpsczofxy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gmxjyjlji.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/goeymfvrd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gqigirqfa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/giiatiffq.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/grqbsvgel.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gvdsaqxmm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gitzyynag.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gzgamlsxe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gtrorguog.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gcdxymlvr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gpaipqmbj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gzeskzaii.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gmveamans.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gkoujztrj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gpagtkdqu.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gmsspyljq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gsdebtfkl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gudshvkrg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gfszxkecn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gaqcgcgcq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gvhmzkowu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gnlanwyfe.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/glunbumpo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/geywnynlb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gfqlvmlwl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gjmkahroj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gyddiwzal.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gynwtbaus.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gsfrkesre.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gfumjmvms.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gptubrlsf.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gyhpdjixo.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gbuwewivu.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gtfqagqfb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/grezbnjdx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gvoxgkweo.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gqkfdxvwd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gztqsxoja.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gugbsrrhn.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gzertnmvr.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gpnevjajl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/guvjuwaow.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbvryqim.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmcjoxgfi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gkhubeaps.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gdutlmawj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gojbcipad.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gjbpufpwi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gusabfblz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gxudbvucq.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gdeurajjp.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gtwvwuutq.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gczwwnmkg.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gebyqjccu.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gzulwavty.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gwyisvuip.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/guieryqpy.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gtlgpnkoo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gqcfgkpdr.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gtrqxooso.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gfltewwjg.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/grtftcwcn.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gryjmksbg.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gxwtnswss.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gpxqiqxmi.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gdadazmar.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gvpbsjnhr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gljqhhttc.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzkvuzout.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glcgjgxgj.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gpokgeogl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gudtkirpc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gbybhdpsb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdugfojbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkncajlog.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdgpgshxk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/ghlprudue.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/ghewmymqx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfsanvbix.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gixjuubpq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gtmcnncrv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gwrjrdyep.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gankbnebb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggmvlnbys.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gfxxgzejq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gevwuolne.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gdyoejggs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/goegqyifw.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyhzrzpeu.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gekguvwlm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gkmswvxth.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gilruqhqu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gpojorboe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gmtyuartd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gzowpmqha.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gagizibnu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gumwysvrw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/ghbuuvnmf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gktzbyjav.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/guvaizjte.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gpyubspqn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gspbjctqy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gmhfspnqh.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gyqwqlkoj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gbpvsdyrf.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gksrkiytk.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/glayprkmh.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gykxrrxse.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gleddxzfj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gzmqmlqwf.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gkzcjtzkf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gcffnqcwv.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gkotlbewu.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/glehaysys.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/guybqwuto.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gnyosrtog.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gtawpoenq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gadznnnil.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gqkjpoidd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gjyzpywkj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gdvipvasq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gzdwzbeiz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gmkjkxkpv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gmtecegxh.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gbammzgjd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/goxglohhl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqycotblr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gpwicfyfi.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gtevigvok.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gltwnjcom.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/geywhlcfm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gflzylecs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gaacupior.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gpprabewb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gqqptbnen.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gjosgoafh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ghhweeabx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gbhzmiqvf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gbapkrvay.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/ghafshbar.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gznfyltwq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gyiqtuyid.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gnfrzwinn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gsezwbxmw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gluftjsou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gokcoqyox.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gssnihbae.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gunbhhnoh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gwscbqqec.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/ggwdqjzom.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gfpgaoqcp.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/ggihpburv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gciejtere.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gkuoyggrb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gfukoyoxb.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gfjilstuc.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gnjtnlrli.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gumitgvpa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/goceenhmu.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxdilktwj.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/ggibzqhtq.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/glnodagtp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gzbtymgrq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gnxvwmygx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gkvbvnnrx.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gvmlaehys.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gqlftjips.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gtcfaaxgx.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/grklsrbmc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gjmnipohr.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gyftuerwr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gvpwtwnqy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gxjljcwaa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/ghmcscogc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gayojnvng.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gaicfdxru.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/geqotxdwr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gzireutfq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gavibklli.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gkuesgjke.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/giozpyhaa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gvpgqeaho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gskpvjmmx.sHtML


<!-- 参考信息 -->