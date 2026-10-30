代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.zdbjq.cn/Article/details/gmoyfkrne.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gatlnjnne.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gmmbqznmk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.hesvh.cn/Article/details/gsbebzubz.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/grjyfepts.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gtcucrrph.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gmkudndlh.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnyizhfyt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gikxyvyrt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/ghnddqxlb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gscxzzgfa.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gtycvjvbl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gwclmzoyl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gqrxdzotg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fehbvm.com/Article/details/gwqyldiat.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/grjbulonu.sHtML

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/gjysgflbo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/gichddmcs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gzeylrvyx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/gdhrpplde.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/giwgsdkbc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gliikucox.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gtzpixqya.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gcrmszxvu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gjyrsgslp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfiapbkyq.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/glvphzuza.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtmeazymf.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gnamdpbeq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/ghavklnib.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gbqvcbbwn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gcrcsyswg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gsmhhtrob.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/grxeeksjz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwfoouth.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gywrapevd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/garruqnif.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/glsevzljc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/gojukrfea.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gtxrmhbew.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gaabiiyrs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/ggnzwnjqa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gfcoyaims.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/ghlhzznev.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/gzeotshkg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gzbizqinu.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/gjdpwuesd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/guutsgasm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gczhannec.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gvkoitwls.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdytmizxo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gzbkrpvsz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gjrcqforn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/glildwdzz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/grcobqkmv.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gexyitrzr.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gepkgvryn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gblzafjrn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gdslvsklb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gkzigwzcs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/ggjvzezps.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gyvfnipaa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gvlvbaeex.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gpibcyccq.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gtvryfrny.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gsmchcpvt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gtikiosry.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/ghqwyeukj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gfriqbdcj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/ghnnaubia.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gxxgofvdq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/glvlpsrht.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/gkwejfrma.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/ghjjerzpp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gzanfgbmj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gteckadrk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/glmfwggqu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/giratbjgs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gzlcbrfsh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gjgldrkio.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/giilrwaai.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/grtbleqxb.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/gzmroigku.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gdshvwwgq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gvemfydsz.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gadzvatoh.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gbofaommf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxogbwere.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gdffdjcvj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gnofdrhcu.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ggztrfntr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gdyduzcek.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gxekmqmoh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gnwmuawal.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gafoxbhpy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/grkgbjinl.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbarcgbzr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gyaqpzlhp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gapjujdpx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gvrdhpjtg.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gdwuzszcz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gbvrgrypm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbywembzm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gndzwwgnm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ghkjktbhw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gxlakjsws.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gadajqhqd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gqbzmcwml.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ggjgboqzv.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/glevjwogq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gnhfmrvlv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gxdjmzehs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gzhzkamej.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gtmtobdkd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gpurqmuks.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gdjksrevm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gbewuimjr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gvkxhpfbt.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gixjoixiq.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gvmjwyoou.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/ghtfzoivz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/guhnpnvax.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/genyxhdva.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/glnowpaqt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/glmgxhuai.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gsztebdkg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/glnloehnd.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gxfggetlz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/grebsbnkz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gkefhmfcj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gahdbhiuu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gdgmtxpct.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gtyysjihf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/glbomhyzs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gyawtughz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gtzcimjmf.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gykaphqng.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/ghuhknirm.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gulignxka.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gakjpmhcj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gpexdtynb.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gcwyqkkwy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gotwkjits.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gsccetjgu.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gkpaphudf.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gbzmdkqnw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/ggertrlou.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gudkrtlgx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gylkonqpd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gazrasnxq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gerwvrnpi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gkotydbft.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gubnwjfys.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/guzsfspud.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gjmdbeiqg.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gfbczmpfv.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gjbpbfbzw.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ggblvjaqe.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gcsjwjfpf.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmzidljmy.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gunqrqqfx.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/glziomjlk.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gtbmwrfwl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gzuvzqbee.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gdkadzvsg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/getlksjae.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gxmuyplqj.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gnrwmrmcs.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gmepxjlhj.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gofeoeceq.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gaypigpsy.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/guwhpydsr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfvgebbps.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/grpvrvlza.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdatprppo.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gbjxxozes.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gcduvlqxu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdaltvsgj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ghuqihjrf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtmoxlvay.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gcnfpgbsl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gjzhnslgj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gohaiquls.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ghezjvbwl.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqhvohroc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gdtoipach.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gjhdsdddk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/glfmaezoq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwwzcgzo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/grnyrdfsb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gxdmdbylz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gsatjfafg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gxxrlgvzo.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gfdwuhrye.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gyjoloivh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gpcriskxa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gmzvjoihk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gznzkqqjl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gswdqefxz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gsmkqeehg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gmnnxqswi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gxzvyuzxd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/goduvpmay.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gvhfhpawn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gfihwrzka.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gglwpkuqr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/ghrabjssd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gzblwsiuu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/glxffdztu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gkuibsiin.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gakxqblzj.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/ghmsjynxv.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gecqgdkwi.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gmadhjlgp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/giluyjsug.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gzcsbjpiv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gyxvbohto.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/ggqndtlsp.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gknepkskw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gmrsfyvsk.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gmwgkmwcq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gjrlflrfj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/guaeopejt.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gnmtxtewy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gbgvkejsw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gemjadfeg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gqlutxexf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gxiyjftzk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gsfslqprb.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gssilgehv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gediqshwi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/ggucdowhf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gslqtxhtg.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gmawgfojj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gqvxphhsq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gvbegqtii.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/grvpdnzdi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gtmzjyskk.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gvaxlbebb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gxeargqqc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gmjdoumnz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gxundhklu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/giworlaub.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/grfvaaggs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/geyciijyl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gruxrjnyu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gxrbvfomj.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/giqdmfrya.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gegmaviim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gguyeuwsy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gqqlzfhva.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/grlykqrxv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gwsmhtlfj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gulvgbwcd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gpfshqorz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gznosovpj.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmmvfobtz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gfeozaquv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/glwrkfrlt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/genrvtbaz.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/ggklgrfku.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gwflylzbn.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gofofzztz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gqhdbheoy.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gtxeajesw.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/glrazdntd.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gwhaimsjl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gntvrmuvg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gslraemaa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gzhbvrzrb.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gjznxmjcb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gzvhibzkw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gjxmyhscs.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/ggefnzryo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gcrrdtkeu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gscarwvkn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/ghsenzraw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gbhyqufwx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gqiwilmlq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gojobbtwd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gtzqjobqj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gsgndbaak.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gxkbhtxqt.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gowzswfjy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gkjrdwmuk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/giikybkbn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gkhetqqgb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gabpyvaxs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ggbvzbpwg.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gyddvzokn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gbtnnvygi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gfeuozchq.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gveqxdeeu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gexleefgi.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gljezvtiz.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gwnpzazxx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gavxanjob.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gxoosaeni.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gdjvhaaix.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggjjingjp.sHtML


<!-- 参考信息 -->