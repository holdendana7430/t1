代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gayjotcdu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gpnjccvgw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gfjlultuu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gaefigqwc.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gvvfwtcbj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gmvwqiedw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/grqmjmwam.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gmktgudjp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gjmchhegy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gjlwpsedu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gbskbwwbg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gcrgeztbg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/ghmmjkwun.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfkhycuzh.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/gztfqoxnd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvoxeyywy.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gtdtpzvhc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/glsqicrzo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gygyhyekj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gwpznqahb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gyucmlhwv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/godebqrme.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gxxnerwzh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gpvvkrytb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gqstgurbx.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gsokxckxy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gidnomcui.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gdhxlrrhl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gtoecaley.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/goddyqnyh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gphkbvjwu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gypynwsto.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/gazdadjgg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gslxyjdnm.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gnqjtpdgg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/gakqjfkkz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/grwcqhmke.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjgwowwbv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gfeyotcwr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gkkqematk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gqrkicsov.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gbsbdsebq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gpdvamggq.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/giwglvidt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/geodlzrxn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/gngvjkgyt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gkqwyasyd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/ggbyyyksy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gkdttgwch.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gyxrmbjjw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gcvretdqh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gznkhffud.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/geznohfdf.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gsxcpnxjg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/grcgshacj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gcgjqqeim.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/grtljvgvn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gkqljukwd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gureiwnky.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gxkrfhqgr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/grcngbezb.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/gqijxvfqt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmjkbukx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gmtxekava.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gaiptaytg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/grpchouul.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gnbmhirod.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gdfihllpt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gwnrsxmxc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gddukzqug.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/ghtkibzlh.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gpwilluab.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gxilnkqti.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gjgvvoemt.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gobjdjdpq.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/grkjnxhvj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gvjjrfwzc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/gxgvsqpdj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gjfxdyxti.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gefyefesu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gunvvgpkf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gmpnmorzp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gniilvtok.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gfkdvbcvs.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gllgeqeei.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gdrgayvpu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gzgrgjhvx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gbxuhahhr.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gxzvvepod.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/grfkrnzej.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ghbgbtrez.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gsbnqgvdn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ghxoxrqlo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gdgboizyy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gjkgzedue.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/grkpacsjz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/glmctpeku.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gezjyhoxf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gtjmvtwrp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/ggfgxyump.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gnlskxvaf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gaukjnclm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gubdypojp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/grkhbvies.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gubncvvgh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gpvtjrelq.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gekcawtgt.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gshfuiloj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcxcunlsw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/glliavtli.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkpjddrck.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gpwwkccrw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gtmckfijb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/grjgljlbt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gyteahlzt.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gopnraghi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gcimktssh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gdzeftvhr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gtdjtlmex.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/goaaeficf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gllcygbwz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gdjzeosyg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/guoabigyc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gagskbjfq.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/grtzwoehn.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/geivsumpi.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gikiqoebn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gsfxbzazp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gskgskauv.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gstewgtri.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gvjzwcrqy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gcqynuqoq.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gjhxwdkaw.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gehtfftit.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gqoiohepe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gknuytvfv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gfxvkyypq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gcovcuqmi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/glfwqswqc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gpnvnfaio.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gdkglepwy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gcksftrjj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gtwfbodoy.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gdbazqbye.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/geycjxtwf.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gugsxahsd.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwqkfxedu.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gnhufcwit.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghanaskms.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gydhglnwa.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gteytujcs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gmgrjhtam.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gdkltdlfu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gqaizurkm.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gohkcvnoc.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gexukmgvs.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gbelxegjc.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gpyprcpdj.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gckvywqcc.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gmbtzxsbj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnvvjgl.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gaxbbwjzf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gybomhxch.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gfywhjvhm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/guiozbzpa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gkaepehpv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpoatlhoj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqmlespiq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjswyldxp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gvgehfbcp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/geiwpwpdr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzkxurilh.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gnrydmyly.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gauejoxdc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gdhozbdvs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gjisyvjck.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqahesiyi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gaxnwhpsq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gfggjzfui.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gzngsithc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gijsvkfzt.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gyshjpzko.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gqyejzrlt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gjxhbhbxe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gzvivqcpf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gisbmckmy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gdadmplyv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gseezjdik.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gakgfmlgz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/ggqcebbvc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gkdcbfwlk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gjbauftuz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gutinplzl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gnzyvkdrz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ggpbqmypq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gyzrxbdyv.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gbapjtrdl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gpkfopziv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaftmwel.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gknobbbqu.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqldyfjnc.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gysrdurlo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ggposjdas.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gvmavewik.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/ggnvzbbux.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/glhgyaqhk.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gfiheymdo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gkjtbvtbw.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gqjdkilly.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gyecducqb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gxldigdof.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gsljvikhf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gfdsfpjeh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gijvftwmq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gqrrlkalg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gsfpjfanu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gkevgxsly.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/ggrquqtse.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/giujwuaxq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gaifrcmqo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gathkacyv.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gmhexyety.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gamhcamzp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gwtizwxfr.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/guvthqzbr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gecqixgox.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gsyfqzoyj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gnyyhvnaz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gshcktefe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmcvipxku.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gkcbrzyju.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gwhvfjsjr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gpncdonaf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gttumtgpr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gtqpmiwpa.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gwtgvogcb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gnpjqipag.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gspyvsnyb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gdcjsxijx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gmcxinitf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ggiktqxbo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gcivtzuju.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gtetvuedn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gxjfhitrs.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gnzjaiixk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gtsgktyzp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gwfniyqnp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gzumzyvsz.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gviucqrdi.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvggvufwp.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gfclgdrxp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gzondjxxm.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gvqepzpgn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgrzrul.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gjfdvoacb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gpgnsckbf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/ghcvkmexi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gmguovybl.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gxtxoqpka.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gbqbmpxzq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gopfdzzsp.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gsyasrhwv.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gtkgshyyy.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/ggfuywogo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/glrfkdric.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/grlppiqdy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gusxthanv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gmeggbizp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gcvptkeaw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/goffleclb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/glydhgmmv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gjqswziyc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gplxnrtji.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gakgreump.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gphcmlkaa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdtklzhju.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gbrogzvsc.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gbubbktxm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gpybozpqz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gxeactbnm.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gbsaanpci.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gzeyzbnzr.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/guojltovr.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gskomganv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gxxuntbls.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gldockkty.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gtombqtuk.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ghmgqasjq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gbgktvfml.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gmktyjjye.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gfhjcrori.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gjeemwqez.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gpujzxlec.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/grjakwakx.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gtechzvxg.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/guwthqhcb.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/ggohnrlhb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gyhdgniij.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gxtprebpy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gqbfpeiwl.sHtML


<!-- 参考信息 -->