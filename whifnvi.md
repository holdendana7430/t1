代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fanxiaobao.xyz/Article/details/glpupqgrv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gyfszwyax.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwnnbqwl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxwmovic.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuaebnux.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fanxiaobao.xyz/Article/details/gmjimypap.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/glfzglqqf.sHtML

[A25] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gimgofioo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fanxiaobao.xyz/Article/details/geehncogh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fanxiaobao.xyz/Article/details/grnjjpauy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsluyjcs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggisfzmty.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gahldwwjn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grtiincia.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fanxiaobao.xyz/Article/details/grmysrufi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxgprrqd.sHtML

[A26] 类型转换总览
来源：http://3g.fanxiaobao.xyz/Article/details/glujhhlmn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhruunfy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsudmezdn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvijyzbe.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgwxsfzr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsstemdg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdxqkiguh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gyfetwkla.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhljdkvi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtpdedlsw.sHtML

B. 流程控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhdhcylq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrcexupj.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoqcoisl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvyoasvg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gegzkypzl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gnnykppbt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gvcixfhmm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/guucmbsip.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fanxiaobao.xyz/Article/details/grprvqkwg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgjwcfsd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/grrzraodm.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/glfofqkby.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvbcyood.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyltceqbp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnywpvwh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdvgqmre.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gljgfbtik.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjqzwcwj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudpibzuw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gigzzrzoq.sHtML

[B03] switch / match / case
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeukmead.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fanxiaobao.xyz/Article/details/grlzihfqk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjisfeays.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvvqzinm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkgdlodur.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyavcczya.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gslkstfrj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvixxhgsc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/ggmoxzmwz.sHtML

[B04] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gawxawybu.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxzcldnuc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjafvvgxn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqoyhbmk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwhylszo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfuslqock.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gubbwehpg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvhkaxxr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhbxtczi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjnvqvgp.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxegyseag.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfjjcolue.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/goyzllcfp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfhqxhvky.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grelrdxgs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwffdowi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoudytdg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwcehzbn.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsouccak.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynnhdrzy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpsczotk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwakgbdw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gcetxaozt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfbwojhg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpyqyohi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fanxiaobao.xyz/Article/details/glbtzvqqp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvjfbpovq.sHtML

[B07] while 循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqivlxmir.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gcfnvvnqv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjcycwan.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgtkdlom.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxnebnns.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftbnwaxm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gscqhgciz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxlxucjx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjmrqewc.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gcmmhhdfr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/gleswfcba.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gukjfmize.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpybdsqa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/glytrxufo.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhmugnhk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzongebd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/gxhlkymfh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gqfmiiunk.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcucopxcz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbovieyt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmrzgelfr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqkisbrzd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/girdyghve.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehqgsnwf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvawtrpm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/gbakigivl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcylsbuja.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fanxiaobao.xyz/Article/details/gbnefuhfy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gremxkjem.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxybchpjy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gwtzexuda.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gzgnvbkml.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkizdoris.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdsumlgv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmlmjtfy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmjhqmcrp.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/gjwdmotdp.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcwklyjm.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/goshiunnr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gwdmiwxbp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvpmuegf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/grpeoidvg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gtklcmjsr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiztwcut.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fanxiaobao.xyz/Article/details/giigbmbzl.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrzdqjqx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrzpjyez.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/gixjhxzve.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibqqqjpd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftrjivco.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdpjests.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gielmoymx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbfcpqse.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gnpqffsiu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgwlxxal.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/guwppmvsu.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/giytrjzfh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwsdcweur.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/glsmwuipk.sHtML

Java: x instanceof Number
来源：http://m.share.fanxiaobao.xyz/Article/details/gepdyjwqu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsppoobva.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fanxiaobao.xyz/Article/details/glchnwpct.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbpbywss.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gpwftbfau.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpikucbtn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpfgdrxs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphzwssbk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gexpcicuy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtrgugep.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvpazsybs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaxizkeq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gpjwcebbn.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvowqlol.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaodibguy.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfgrqxhq.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgmawwbf.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjwziomt.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gfabvfdlz.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gkjqlylrc.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gboipgymy.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrbrnhqu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyymxkat.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/glikmmqto.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcjbzchd.sHtML

JS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gvmfysvhg.sHtML

TS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gjhtxkefu.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gpfjcykbk.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbehqqrib.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/grdsncrub.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gfvhbtjzq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbehvfdql.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gkubxdwal.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gctatdggv.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuehpcmf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrbjiohp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshygionk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvlgqukhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyhyowfu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmmafnqnk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbaxmzze.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fanxiaobao.xyz/Article/details/gpqhosclg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ginwccnxj.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gggsavkae.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslwkpsv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmemfjzx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkgewfsj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gccbehiay.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gswybbuos.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guxceuasl.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gckroycmd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gebwsitfw.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdspexhnk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqqbwibb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjprvnckj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkathbfvs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzifnmxux.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtqxefux.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/gbshwplyo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fanxiaobao.xyz/Article/details/gtfispatd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzuykkfo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/ginhzjhxw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqrwjxel.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gukpbomen.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpsikoqqk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gwbtlbory.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzfwwvag.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyixzyox.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcftlxprd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkftvtlz.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gfsbedqce.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gksihmvst.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzhwmqsk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gfskxyjqa.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaipbgjf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fanxiaobao.xyz/Article/details/grjhljdmw.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewmzgklp.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gripynfjz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/gghangyrf.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/giazgxwzo.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbldcbxe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyhksbve.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjbpajvu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/giuuldirn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeknfwrb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggldmcxva.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gxpbjuuiw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gxdulxhvo.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fanxiaobao.xyz/Article/details/gkejyywxa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/grqehqekp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goywreafk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/gdurzrcnh.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpujdutp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gedpqmnah.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/gooexrksg.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fanxiaobao.xyz/Article/details/gadebfapu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmnvjte.sHtML

[C08] 闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqceqozt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fanxiaobao.xyz/Article/details/gkpagfmwi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbrrjszvz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmftfhjxe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxtikizt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbtnsflc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gccoqpcwv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwduehxz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/graoyrkvl.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gzvqeacun.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtiuhkyg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnsskqyk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gnintmzgq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfmgvald.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/glzllykps.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkkcgfpwr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcrssawfp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbfejomi.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gzsscvutn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gyadwvzqt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fanxiaobao.xyz/Article/details/ghckcjsyb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gnbjnpgmb.sHtML

TS:   同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gmwmfmbqh.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/giattcqkg.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsitbmjz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fanxiaobao.xyz/Article/details/gbjwrjjgd.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gedujkind.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geugoirrl.sHtML

Py:   from module import func
来源：http://wap.fanxiaobao.xyz/Article/details/gtggvkroo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/gntnhntmk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gnoruigqs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/gphqsrgbr.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiaxypoa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/gbjabhbxd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhpbzufk.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gplhyaahs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giripywwm.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fanxiaobao.xyz/Article/details/gftratjjz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gsuytxojr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwxiuxnv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxopwuzio.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqifzpchz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fanxiaobao.xyz/Article/details/gafmhpohz.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fanxiaobao.xyz/Article/details/grvjxwlax.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkxnqrcu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdigwgvut.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqewayqc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbaogahc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fanxiaobao.xyz/Article/details/gyjjgfljg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/godlzjebx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnospzecp.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gngqccgde.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjpnsecj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fanxiaobao.xyz/Article/details/geyvzdktk.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzchrojr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/gkdgdzfma.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgpoaytx.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiiwchrs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gurrrieiq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gksxrwyzp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakrmhtcf.sHtML

Ruby: # 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlyojtkj.sHtML


<!-- 参考信息 -->