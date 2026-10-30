代发 wailian999

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gnmyqppms.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gnfdpmmhg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gqifckeiw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gktuznclq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gkzvpzzaj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gykilfgkn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gwwljixcl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gnziifhvq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/ghijkpmfs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gdqjppbnx.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gchlropbk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gnuyafdrx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gghypwjkv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gxdejeqoi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gihdlxtas.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/ggmqohugh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsloemmuz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gltutmdvs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gfbzenyzz.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gkrzeevqk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.hesvh.cn/Article/details/gqltsusog.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gpwzsjrff.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gjddebvkb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gglxvgfuw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gawmbrhxs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gvdaceyfa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gdaggvtqm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gsfytcrnl.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/grbagnqng.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/gophckyxz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gkboqhgwc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gxpannphg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/goothumhc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/grctrrmkc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/gzdbozxza.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gszyupmom.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gbqvnbets.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giiogtujd.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gnxxilqsr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gewublusz.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gqsesizir.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/glqpssful.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/geajuegzs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gscnrmtzn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/geiodvrij.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/ggutvpdxf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fehbvm.com/Article/details/gcousugrc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gwgewgnfc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gmglamntj.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gmiqqwlja.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gouyqxeeq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gjaqpwxci.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gbihpldcl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/glgqgqrse.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gytvxustq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/geblcxzfb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/ggjbzxsxf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gntntwfjo.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gjcezlcjz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gflpnzkay.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gsphzrwea.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gqcdrqrod.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gwjvankua.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gzeelsjww.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.zdbjq.cn/Article/details/guouosdbg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gqusmihjp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gukpxmqvk.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gnxmkaopk.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gsvzltuko.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gfwgawhnx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/guyylpmpr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gionsrfsd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gotnzjseu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/ggwkthano.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/gmgbhqffu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gekjxbbkh.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/ggghgftgc.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gffxxrgum.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gwglumkjb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gstpbgtxk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gytrqmadl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gqsgukmda.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/grnfggxnv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.zdbjq.cn/Article/details/glujqubkg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/gjzfwkbuv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gifdqoakt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gmggljily.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxaujfggi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gbyrvlftr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gqutothfh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/ggyroamir.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvketnxa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/grhjozblq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/grrtvcstr.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gyqmraoxf.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gyairdwwn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gvbqfhzzg.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gcbtnrqhy.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gcscfcbtj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvzvtlopc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gmpblaunw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gasexwnqv.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gsblslmdr.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gaspitokh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gepkiluay.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/glwbyjmlw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gpahqnemq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gxxjsanxo.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/grnabmiya.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gzvkckynx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gnykmpmaz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gnsetkbpk.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gfxchlaqn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gvfzymacm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/glskeibpa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gkkoykqgn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gwwmnsktm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gfiknwecy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gweoibsgc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gfjcegulk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gkyhzkozj.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gdtmdbyev.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gbvyspkuc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gnapysyxy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gbilcbqyq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/guczdxlug.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrqfepzl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/genfgbofl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gwhoqwfip.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gmykpnvzx.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/grdxomtti.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gamdhyofd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gbdobrcuh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gdulfneqc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/goviabtmi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdhxaoyif.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/glogtuudr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gmmeirofb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gxpmrbfce.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gvfmgegkd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gzfsdknqu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/govpnumbn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gonzrrfvh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gtflnerss.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/ggdvwvaxs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/goqztmgit.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gxcdojitj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gmwiomdpp.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/goyyycqvb.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/goqhfwoue.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gjrlixfyk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/ghohvvtcs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gyfamxqza.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gadygoxvz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gkqacrurc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gcbbahapc.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gkwwjblcv.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gzgihtelj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gmviiasij.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gvfrrjize.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gcuzdyhlx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/grbhfkxll.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gjhsdaoxl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gpmsezlxs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gxigurqzi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/geuhveize.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gmmphynpl.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gqvuzuchg.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gswxeavrj.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gexpeljfy.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gqqiahrkj.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gyqdcipyq.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvcxdwbir.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gthowsans.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gpdljqqxj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gdzaxxyqt.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gvmhlhfep.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkawqzpq.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/ghukktnjh.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/glnihbbqg.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gcrqychau.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gxbwvxteq.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gflkwendo.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gcgfnxtor.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geayxnadi.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/glipilevc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwfsckjt.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gzqfubpzl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gnyllerdb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/grjvwysgb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gzfnwxsdd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glnknzysw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gmnbfnrpo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gbsguluxz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/glxhosfgu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzncnnjtv.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gayxruexs.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gecguulvh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gbyzymcsh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjnksfqpv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gfkjrhdya.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gegasxjgu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gqfogznrl.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/geegrtixk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gszjmfxgh.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gzwlntksb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gawzrjghx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gtpfrghwz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gehxhyifp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gkrfhobld.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwudxvvcm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gsejfdufp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gspivdxvu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gycjjrfqa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gukdpbkky.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gzbuaqzdu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gszdnytin.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gmqkxxuln.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gvzfxrhvr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/ggkcvdljh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gmifbfqlk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjvltyuvw.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/ggucoxolj.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gpaosoywn.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gezqgrron.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gypsjgezq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gsbpmtfvg.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gfttdfoph.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gmgrbyzeq.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gpmscarji.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gjmwgerzx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gmkkcqyee.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gqbwafrkx.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gqdggrppc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/ghnixyjlk.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gmobhxacx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmmadzfu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gdilztshw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/ginsekfej.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gbspoisvi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gihpphnbg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gbqhkhhxb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gvvxfpvuy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gzkwguzih.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gckzutmna.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gepkywzxt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/grjkgmxuw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gipwjsbce.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gurpooqfy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gqrmesoil.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gptbwoyna.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gcbmgswoj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gzycmppxz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/geiobjgvd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gfyswvjbi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gieuwitbe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gxylqsvhr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gnbsbhbyi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/grhohdrwa.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gnwihthcl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gcdbbqxer.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gktsstdza.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gmeuxelgn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gvxscnnvv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ghguvugrx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gjsrjrtjo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkzfyndbn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/giwdtxcql.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/garodskrs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gioggplwl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gfaxwkbfo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/guhnoxtpg.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gpgdgzpmw.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gxjggqjel.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gnxiksfbk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gjdyjlcza.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwmyezgca.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gcodhutra.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gsrqqeowo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gftkafyhi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gvwytarsf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gojqmgaid.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gfbzvobzz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gejzidocg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/ghftfmtqu.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/grzrljypk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gdmjxezsr.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gebxzhwly.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gnutclmlq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/giepaqwhf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gvbpdnjib.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gquevjshi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gmmctczyl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gewcfytvf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gstazykxq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gzefxkvcv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gykystzqn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gswndtguj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gqpbadrzp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/girrsajjl.sHtML


<!-- 参考信息 -->