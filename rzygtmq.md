代发 wailian999

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gltkblauy.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/glffqhngb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/gvuygeepe.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gtgpfmimd.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/ggxhayebd.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gcmwcaojl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fehbvm.com/Article/details/gzvhpradh.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gbjeoyxse.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gayvepupk.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gcnzgyadl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.hesvh.cn/Article/details/gjtdchnsg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/grduevcoz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gdhsqqyxh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gsymwvnku.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gfrrtnpms.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gttnkxdhn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/ghijlralc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gpycozjqn.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gpjsekoaa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.hesvh.cn/Article/details/gthtboobg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/geebzebxf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gpzwhmmvu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/grbjovbqy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gtryloini.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.hesvh.cn/Article/details/gndxwtfee.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gcyfifcbc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gflvfurrt.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gojdffhrr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gbslhzcay.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/glemzcofh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gdoezllho.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gngsiudur.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gnemzbrss.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gehervmql.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/gwgjtpdxb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gcvqskhix.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gihzsfbpj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gffcjdunt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gtbstshza.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gejpdnbvl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gvlbfwwit.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/giyvdcfxw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gpbfddplk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/gvzcgggip.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gujmjugdy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/galczvpms.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/glwlvozdl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwfdeoztb.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/gdzhjalxr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gbarnccak.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/giufbgueo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gdemmpoqc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gatfydqgs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gcaqhidmo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gdrhjuqvd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gzkaekygo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gkjjqqgrt.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/ggittycpo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/glsaxwtaf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/gnzvifjbz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/goccaxkhl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gikegnuhc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gxpqfhxju.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/goclkgwfs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gmedserhv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gyekajmon.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gbbhjhiyy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gzamuainc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gphkhsehz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gpanenhrl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gvtxefhmv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/govijpaqq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/glpvodisl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gnwjftiaw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gcvxtwhyi.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/glifnhnkd.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/ggbzixjlf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/giymqnegq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gcyanskbx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gfhkclzxc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gtbpovhzu.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gasjepzzd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gllgsglni.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/gcjzbaugd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gsntsyijk.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/grmvdskkh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/ghyfgxcbk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gcbaxgjes.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gqmpudnaf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gfxwyiwzz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gjbzfzuus.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gjojiwwsf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gptffbfat.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gzolpzjze.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gwlpbajdb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/ghrxygvjd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gsnnzlrry.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gsihjkjbg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gorthwmlf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gccgblhce.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gekczlfcx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gbbefebhh.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/gqljervta.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gbdpmmuus.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gxlxeltvk.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gnwxxeadh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gslkybepu.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gkhzhnmrk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gsrzddunu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gksjmtbma.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gzbomhbep.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gksuypdud.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/grzpqvfev.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gsgcfxpxz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggpodhklb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gslqtophf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gcjabchmk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gzfzjowmu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/goldlxtka.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gcewujleo.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gapdazwgz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gwgkezvvc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ggiivctey.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gcfwojjhi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gqcmwfeoa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gxecwzeng.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gldjhlmiu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gdnrhymij.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gujdavriu.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gwmnneqzh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gjgcrevmp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gjbknoiag.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gszbkyusx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gvziejiga.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/ggrwqhqoq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gxwnucjcg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gtoebvpby.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gzjnpcslo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gllijmvrn.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/ghhitvzxu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gioptutko.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gsheyhboa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gapgyuune.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gwhiktctt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/grpwnyqhr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gcamxmynb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gbruzynvr.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gbuyiycdi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gbjudeihw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/ghrmyzrer.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gtrxxcrcw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gpexlvlul.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gkpawpxak.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/gfaemqvcd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gqakwborr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gzajvgpsp.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gutzdcopn.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gvclvieco.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gzwvaxfrh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gmhphxbve.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gtxigfxnk.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gzicvfwrq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gufprpjxh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gsaqtcdsj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gtdjddadb.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/growgbvdt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gfxioxhoh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gpuqocjny.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gyclwlspd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/goanvmxpo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gurddptzz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gproxxhwb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/ggoyxbgjt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gziwxoxjx.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gpndobawm.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gjivnyjkh.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/greqjjjxl.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gocjgjepu.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gbmtcyhsf.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gycezolav.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gkbxebzmv.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gysvhvuxg.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmqasrufn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gbkwwsaip.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gxzpjsaec.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gubhhvfee.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gbykwctyk.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/geicwkunx.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gfzvrlbsv.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gghtpzxcg.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gcdhwjljt.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gycyhxnbc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqdafhqwo.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/ggbxrppqk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gumamreje.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gaixowdpr.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gdsicplqi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gclvoekbu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glwdesrzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/giqnbvcxv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtxnkywga.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gsoqxharf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gujiotdnw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grlvhmuse.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/giumalrgd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gumxkwrxk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gcmygniod.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gterzzbht.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gnvnwxfex.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gwmibmuge.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/ghhyjjqwh.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gwnnkehbm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gucekfvve.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/goedznwim.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdrprnt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gynyukatp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gmvynsmqo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/guhfadfed.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gucdnfqeq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gwmtkwnrb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gpvlyxjgo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gelvhvckg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gqwxbdtww.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gazxijlpo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gqkzqjmyn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gtsbejcmw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/ghtfyumck.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gtofduahw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gfkvhwplc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gmgvvlkwb.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/geqtgcdai.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gmgquiujo.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gqeliakjf.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gqwrpalar.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gihdqpccj.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/giiuurwwk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gruwsixht.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gbjsokmew.sHtML

Ruby: return a, b
来源：http://www.blog.fehbvm.com/Article/details/gqlmzsrmd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gnozxgylz.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gfyppruya.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdjncbb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/ggjhflemn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/grclyljje.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gdtclqywy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gwrfsotkz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gnbozmzzf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/glcdadwlu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gdhkcpeit.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gnozlacvg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gltytdezb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gokzjxsel.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gdcpzqvbb.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gqhxeqvtb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtggbvybl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gfuqcrwps.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhrwrkve.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gnvfeqygi.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gnrzelalw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gwonilfzn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gybhyymja.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gyydprfbz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gpikkrwoi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/glyojprcn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gshatrenm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/giimrpglk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gpwaucnbj.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gbrnywflf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/grmywliar.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/ggohhtrzd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gvmwhkrcv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gxosgweor.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/godjabpai.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gropzxgtw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gucigckni.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gpqfgfoeq.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gneczjeuc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gqtgagxpp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gewjoirph.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzfaukxdg.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/ggvzhksqo.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/glctywowq.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gafmmvjrj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/giofhspum.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/ggqowgcjb.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gwdfwvdcz.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gvuewhdea.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/ghgicjtxo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gngbvrjig.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gwrnewtlt.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gvyiwqvgr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gmwfsnlcp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/guxqknasq.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gelddeaxc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/guyygolim.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gcdrtbiyk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gqesidjrh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gehmrttiz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/grosizueg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gvqgepagn.sHtML


<!-- 参考信息 -->