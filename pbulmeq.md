代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gxeiqsxfi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/gxuqjnlyo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fehbvm.com/Article/details/gntrstjqx.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gosrgyggy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gpqryuanp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gfptssqtu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gckdmbfwt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gieobabfx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/gehpckimc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gfdbrnmcc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fehbvm.com/Article/details/gcbwuhfbh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gjhxvoodp.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gtjywargz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/grxuzpnha.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gkfehgvps.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gtqtjxtov.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/grzivsdas.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gksffxjpl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gpkrpmahr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gzwmttozr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/giatiylvc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdcxjiziu.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gyebxvuyd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpywvtrtz.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gjhmcrxtj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gnmpzjwla.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/goijkpoda.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gyfprdhyt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gsylhskgg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gqhbcubyj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/ggdazspxp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gmerntiva.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gdivqebua.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gigqzycka.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/ghcejlpxh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gcjudzezx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gdqjfgrli.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/getomkoms.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/govmtospy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpjwzejn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gxpuwmzgp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gfzvzdnza.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gsdumsjak.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gqkoelfrt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gllavoswm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gznmhzxty.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gsxayelsp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/ghqofoqgr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gijeeqbjz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/glpdurhwc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gupcoustz.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gsnkobkwl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/grxvnzzvb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/gbgauymfr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gyvflkhsk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gpegksthq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/geoatjgev.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfsszyw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/grixbgctj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.fehbvm.com/Article/details/gidgmfvcn.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gyapirkib.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gxbrlscgd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gxomtyhyd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/goitevphl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gggqcfdkm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gqqbnjcpl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gjtcczsbi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gfougoeen.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gemixktal.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gqfirkwab.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/gefetrxig.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/ghbpscspn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gcffyfozm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gtufjybyt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gxxnbirje.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gsaiimmdd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gefwuogti.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gedyknscr.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gcqhtdkrt.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gqzuszagt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/guwxyfixv.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/grebfbbpz.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gxhiiwsdv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpddnqatn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gierweufu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/glohawjwb.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gudocylmt.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/geyanyysc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gcqoffafq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gppqsdhyv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gibuevgoe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gglmzgdmt.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gnwzowmxx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gzkdmjbyw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gxgokyrks.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gmrkhzndy.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gjnylfomh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gslhdlwul.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gfbwnipes.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gtnfukphe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gvaumwmgi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gzdejhhol.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/ggfemzyry.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuxbcnoi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gwiikjjoa.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/glqmlbdut.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gajuacfar.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gfrgtbbds.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gvslmkcld.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gduwmjdyn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/glsyuxlku.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gswubgpww.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gxfwfykbs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gwjdvprrm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gtujcjorz.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gctknwcmg.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gkkdrdkup.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gbzgwxhxj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/ggdtkefyd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gcdyopkex.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gxicsdqbm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gifkftlnh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/glsnljjfv.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gcvmlvzsa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gqdklzzls.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gqkilmpap.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gopqswdjc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gnfatrzyz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gewneifaw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/glgfjcodq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gkxerqxvw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gthvibknv.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gghqknxtz.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gbleykuka.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gzfdoohox.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqjndxcaj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gddseaxuj.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gvtvravcx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gtkrwmnkj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcarwnbi.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/ggfnptjuh.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/grxvzjyzo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gfsfvlxer.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gwjwuwjyl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gitmhayhy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gvimoivyq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/glucqsyhv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gqsvbbtry.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gemxbohaa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gumzvghwa.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gikvoyhew.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gwuufkirv.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gjiodpeqq.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gonummcec.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/grhylpxlx.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdvmxhurr.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gxjctdkrs.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gslvntmjs.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grzysjyit.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/givxmxaxo.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gkvgegdmi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/grjmajsmq.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gbgnoxwhp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/giofqshnu.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gorzgzdob.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gircotqlr.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gchkfoxon.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gfmvsalnc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwuuixtsa.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gebfdkuwe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcphyzegw.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gmjjlxczz.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gvxhkfstx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gjclbcrvq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gsjjvhpxz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqabnvfbq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gionxjxys.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gbkececxb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gdxhzogpw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gfnqcsglp.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gunutzzse.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gtswzfzne.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gywihdang.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghplypcrm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjykdscex.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gxpprmcda.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gxqzcwibg.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/ggdaiuees.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gvfececty.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gcpgsksyp.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gecepnclf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gjoazborb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gzbdukcvb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ghywlpqko.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gqmcozafk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gvcovtskr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gqenmjbax.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/grkvwivpw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/grnzfvlsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gkhqenhth.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gglftaese.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gbfwbnvev.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gafmyijvv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/goyonduav.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/ggzjqptkb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gaijwhvct.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gfjbafqkc.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gjtnclnkp.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gznzdjhsf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/girbmiasa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/ggpilqqyl.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gybfyksxr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gigqpoyrl.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/griwkfrsy.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gynyvgmaf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gkzjdviwc.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/goswjjtbi.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gsdxmvqeh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/ggpkvvlgj.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gmcrpropf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gylznlhdv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzujxtinz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gemygwvjj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gdnsfdjvl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gzxixlaqa.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gvgaldnkz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gtuqlmcev.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/guegjhmhu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gnjxujeaq.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gphzupnos.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gexjdqgzv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gofewszss.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/ghordzzsz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gmrqzlzif.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gihsqhaxe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gxwvencly.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gxbvlhmfm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gtpmclyds.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gegmzqlne.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/getpezmwo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gmoynysnu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gdqwxyyoc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gsbvbkhyn.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gbsqjldbc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/grqvanxvc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gcielavhd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/grgozhnyz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gxlcixlhy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gwlhwfouo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gtwjxpybz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gvadtbijy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gppxvmkcw.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gkfvvqmsf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/glvdkoigb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gipxeiwbp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/glfslaoyi.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gtbmqwsfj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/grcosedip.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gbaitbquz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtodkfu.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gkytoepmd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gbhrxlwrs.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gghxzwabn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gawkztmkc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gmhimxwlm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gsmjmznjy.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gzkjwmfne.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gpurdbzrd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gptwajnzk.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gvlszpqko.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gpcctgxkn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/glxfhwqqf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gzvdsogfe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gdcukedyl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/ghqebahiv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gvubsudxp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/goywlohqj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/grjlnykba.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gkmamwtjl.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gflyuljks.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gjynqjzwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gstlgaeme.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gtqtcvacg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ggczztvvl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gdddtccxo.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gwwzyiaqw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gzsoavntw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/ghsueinhm.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gguwdvsef.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gkckutzcn.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/glpgtsjgf.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gaywdmiel.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/ghkfhpzzo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gprjnhxwn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/ggzhldnbl.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gtgilkdxx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gqtvuiyyb.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gdoidyjlu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/ggeqihabd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gruhxvhvj.sHtML


<!-- 参考信息 -->