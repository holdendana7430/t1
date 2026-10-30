代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://blog.zdbjq.cn/Article/details/gnyurwwqj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gcahwzqlg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gvcymurry.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/goiwtwepb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gbnifuwez.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/ggccqwlrw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/grxjwjjad.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fehbvm.com/Article/details/gcvrbblwn.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/geqpeyqui.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/garikqrho.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/gizwzbhrm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gapyeaeov.sHtML

TS:   s.length
来源：http://wap.zdbjq.cn/Article/details/gaweouecl.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gkvfegleu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/guwksluew.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gxnwxyqle.sHtML

C#:   s.Length
来源：http://blog.fehbvm.com/Article/details/gjdzanijy.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gtmglultz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gtrucexde.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/glclmnjyy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gbfwzhgwu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gbndedujn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gbxkvahsm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gnreihqjg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/grvgitiyb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gwowmtwwi.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gutlvrvsl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fehbvm.com/Article/details/ghvbcleae.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gutymoxzf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/galrdaevd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gqoprllgy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gxszfgjdm.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/ghameahsb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gpkfcfhgx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gwxwyeadn.sHtML

[A25] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gxogchguo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/guznfzurs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gbegavhkc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gjtecofkg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gdhnsofsn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxwvnbn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/giqoburnw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gwdzkhwlt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gacbghpcn.sHtML

[A26] 类型转换总览
来源：http://read.share.zdbjq.cn/Article/details/gelgvynqt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gbxogafjd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.zdbjq.cn/Article/details/guvtlwqir.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/gdyplvclr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gobldznzc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gfqxtpcxh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gpxpphxqm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gjiwqzhle.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/geobgfgip.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfsqpxrzr.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gltoeepde.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gecgccwmc.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gukjvqxpm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gbpbhucmr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gjkzgpvug.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gtyiaxlhw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gnemdcudb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gzaqfpukb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gordvmipt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gjmzxeyhv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/giqgrqtqm.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gntqqilll.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gnrbakszp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gqesvwsvw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gutgmrcun.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gvyamlwko.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gwvlpmrzc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gjdxfmodu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/ghmeuzpry.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gdasoyjcf.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/gdxtxyfqd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gdocyzkck.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gbmsitlca.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjtjkwttu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gglrlomwv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gkmamymvv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gthjhxksa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gqreakaiw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gzhuchrff.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gizejewap.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/geltmxmfb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gogtskpzz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gvjnfeltq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gmsapgdcv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gfakddwgr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gnvorutew.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhtmxjzk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/gjfioootb.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gdckktocm.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/ggusoiioo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gaacluoul.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gqwaszbrr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gckntksam.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gcbifvhck.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gwwrrjjyb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gebapxnch.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gxdeflpyw.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gnxdotjat.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gkmihxaxw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gxxycagnz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gtqglonyy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gihpyamnc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gqtofpuhq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gtterhegx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtoscwhtf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gytejkirr.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghkhbhzzh.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gzttckuxy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gdzsffheo.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gsvocurjx.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/guarghvdb.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gsplsnard.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/goilggaum.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gwglnhovd.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gdiynwkka.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gryzkljay.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gbrdxvhln.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gcygxxgwt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gxrziiatk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gsydegvli.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gphzdumqn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gopzbrjff.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gxlvdlluy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gkqyolmmu.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/ghihjulhq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gkyvhmifk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/galjkphym.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gaskhnhtd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gptqcoyez.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gmrpaahds.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gabozjtjm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gshfzxmps.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/glknizewe.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gptpeakij.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gmuswcwuf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmrbxpoi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gmqymkjtz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gqmdxwfmf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gyykeqard.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/ghjkepjzm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gonclawow.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gtkbrfdeo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gvjurqfed.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gezdhlayg.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gcsowqlgm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gposwvtnl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gkvjkooja.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gqyxzhxpz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/ghxxkeyri.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gbquentqv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gutjybtlv.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gwkxervgw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gzaoynuhg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gvfnnqthg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrvcvwsk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gvrklcott.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gxyavzimy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gwcibphsi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gwlymugwy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwanhbs.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gtnhqarlj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gmppfbzku.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gheaqrzoa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gabtrkpzs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gkqijrgzj.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/geauuiydu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gekqwqbix.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gvgrrvvmv.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gzyxycuvb.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/guvlzeram.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gdakeewyo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gapgxynja.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/ghxbncyvx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/glzampyqy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/giosxgvbd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gbkivzxcx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/grqbhbpbl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/ggfbkniac.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gkzydzpuv.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gefozpuje.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gxagekofj.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggayvvzcj.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvujbqlyf.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gpsaiseqc.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gjmicgxix.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gsnjkmtlg.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gmofdbeev.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gmhtbkfgn.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gtkmlsdvi.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/guqzxzoab.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gpmtpnhnk.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gfhdrsobw.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gtpxtwrbb.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gxddccdnp.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gfymtiasr.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/guzwtjruw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gstfmrrmn.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/grzqkulln.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjyynjwry.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gcaccxpja.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gqhtbgvjf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsubyvxxp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghayhbjsb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghenmgpjt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/ggzuujwsu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gcdwdfvno.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gvdgcoffu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gbwsgtndp.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gojljuzkj.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gegdgnmht.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/grpjtiekr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gmbfrmthi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/grgepbqor.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gzxinwnpg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gzlddsxvl.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gndnkowzd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/grcntecbo.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gsujdgqkm.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/guoyyafax.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gzuthyprm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gittascfz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gtrswwbln.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gciaseqxb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gxqvnagqk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gvkipblyb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/goynlifwy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gohsjaoxh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gekexodrl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gtdkgxrsu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/glhulecks.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/ghmgvtqgm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gpdelkvjl.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gkznxvyaw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gpafawkgx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxfsqyshp.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/golirsosd.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gpybwpgzo.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gflweowpk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gaqtsvgrs.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gfswcxbgu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gxmdpndqq.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gdgrjbhmh.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gkigqgkrx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gddaekiun.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/girbcuyqo.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gfxjfnqvj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gixmrfujx.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gyfsljwom.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gcqthovtz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gmfjbdprk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gjckjejqk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/guvhejced.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gkgyemnsq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gzuysqlvs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gtxknbuqq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gskbnrfgu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gyymxnxsm.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gdpnihftv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/glzitivbi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gtmluanmo.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gnmbjyodp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/giipvzhve.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gfcigfkec.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/ghgnafctp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gpzhmjxes.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/glwftwzru.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gfjdhyvkx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gsffhveqd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gpfntrbgq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gjmlcpqqy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gcfuzdqbw.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gaefxqlvp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gzkcjosda.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gidgbtswg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gkkttbmak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gjkhcwwlx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gsmyhxmeq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gtexqchbi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gxlrnjdos.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gwwgemndy.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gvvxgpbhl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gaugudrww.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gsqqpclzc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/glshtxtrt.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gnntpzzcj.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gugtexdap.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdrzhmvfv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/goyymdfdf.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gjambgmog.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gwlpomebp.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gpoxyfwcb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gifthpqwm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gxagkdvjc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gegjlsclc.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gppgsysjg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/ggaygxzha.sHtML


<!-- 参考信息 -->