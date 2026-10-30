代发 wailian999

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gwvceqhze.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gefevfvia.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/gfqijetcl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.hesvh.cn/Article/details/gkjxayure.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/gbbwcegaq.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/giykuuezr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.hesvh.cn/Article/details/gphoncfzx.sHtML

Ruby: s.length
来源：http://baike.zdbjq.cn/Article/details/gbclcavry.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gzpiyczbk.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gpmdadhuu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gszbcukbb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gvpxerpjp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gthakpwxn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gzqxvhkmc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gpevnjibw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gihjwxsxc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gssrxbera.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gzoupncmr.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gpeynmzyc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gzeounpky.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gwoxyapqf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gfssfhonp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gyjhstrbk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gtrzhzrcy.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.hesvh.cn/Article/details/gzvzxlplv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gxeksxrkh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gabwsrwcd.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/goknenftr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gpnbydvqq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gslffqvsh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gjpllhmpj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gwrjdhtrh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gniaazmkg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.zdbjq.cn/Article/details/gotgnzefa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gpgoljxnn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbyoenen.sHtML

[A26] 类型转换总览
来源：http://www.blog.hesvh.cn/Article/details/gmvlmpeol.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/goeogoamf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gsicbzgty.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fehbvm.com/Article/details/grjqtodxw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gqolbreil.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/guxdvhfzl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gqdjmbgmv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gsjpvjgfv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gpuahcdvr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghrunwxcd.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gyaxkntjv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/greasjynq.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/gmkijgznf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gounqbqcp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/guiazyvfb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gmywpsvkc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gqzvwpzlw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gijdbwmxz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/glsagqzky.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gjcxwddml.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gmqudhmbz.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gbzwpilqd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gtuxvuosr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gfieeoqwx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdzpbtn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gybjjmsix.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gnblgakjn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/giwyixzeb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.hesvh.cn/Article/details/glgjduqig.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gfdxtwbvx.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gtdcoupoe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/gxgmoxvsz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/ggusvauzt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gocxkhler.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/glgacheiy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gzfvuquao.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gcgfyfxei.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fehbvm.com/Article/details/gugucpzdf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gftaxqddu.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gjseodstm.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/ggnvaddpb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/guilojham.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gcetyoiqq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gsbnctgxa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/giiedsvze.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gymrxjels.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gcyhkhmha.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpasyenv.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gmvwpyxtw.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gzrzzggmf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gttqjwzpg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gwltxqfnt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/garmbsrhv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gcxslfzxn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gprxqilwj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gkamxeuvd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gtizaoefj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gkonjogqe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gkmqbzvlj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gyxkosvqi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/ghmhfhusr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gkhzprfck.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/grviyfzpc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gfwwhppls.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gcbivlzje.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/goxlleocp.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gbxnvokit.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gxysmnwjc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gykrambmf.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gfoukzpja.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gdqhgclgm.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gvyfnsaxe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gmewzkspf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/ggiynxxfk.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gbxcqbsjx.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/guhznujay.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gepopfyzz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gvxzsqubh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gtkwntolr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gccxvcsoi.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gtizsjxem.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gcpmmwjax.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gckxsrnfx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gnuvxuoln.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gsvmioxsm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gicivcizg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gaibozscr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gemjbohpi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ghvjoqkzx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzbdsehzz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/grohtnbqf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gfejxizta.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gppslxrwy.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gdlnsxabx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/glczdgjyn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gyifnmdho.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gdljrmjch.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gwlbnfjdw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/grwjudybx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gnrsktsjt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gkdpkbgic.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gkiwsafxl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gcfcucvec.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gsphzxhbv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqviuymey.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/goxgjfpvz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gwqfhtzri.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gcoloebus.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gpvzjlxwa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gjvkscqzy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/grnlumuuj.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gilwvkedd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gifltrccw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gsxgwkzbn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gyoshlivo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gzzzxoejn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gxvzrzfxo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gkytgeirg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gqnfnomar.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gwsjbwufe.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gldugcdcc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gzwptxflp.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gsaqpamqz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gyhqqqulh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmoxktbfj.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gjrrizsmx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gkxubmwxe.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gfyhrwrtw.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/geojrcvyk.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/glbuxzfxk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/givucdnwo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gfanuhvrp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghqcojrxj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gpmloykuv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gghtyzzyl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gxmtzgdjp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/ghrelfgzi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/goyulvmay.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gjdgczvqc.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gnwmcfxvc.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gwmvhcguf.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/greoyhkxd.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfjxlheow.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/glvotxofk.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gvdgmqplu.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcciugx.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gmvmsjfof.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gxunfjaaq.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gtrptbhnw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/grhcallka.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gygfjsylc.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gelzscpiv.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gcrngytdz.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gomnmgfjo.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gfandlcfq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/giksbljcj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gielnvaez.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gzxwxzger.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grsqbwmja.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqlvidytt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gfvkkyyoi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gbmmnmlza.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gghnohdio.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsddmpntw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnbavxdlg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gohglelfl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gmwzjwzcs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlvpnins.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gtrskbpya.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gtmdxowni.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gcyltbypg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gksnhkmlt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzoieoerr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/grjtyzimg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gvicpuypv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gietisdbn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gghuwxhfq.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/ghczecphs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/ghociisiw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gvsmlizuq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gmfpcwmxq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gjfwjqlgo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gkkcwvsvq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gyztdtczi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gerjznaml.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gmrrszlfx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/giljajdrx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gwtovjpxj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gfkkabxem.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gdbbgspyg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/guxeihcyr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gjrlwsyrx.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gsdwbdaib.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gexwdfabz.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/ggrwrtghl.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gxjaupfom.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/glgbqvbza.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gubuplgnd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gzhnlivee.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gyqnurexk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gkwumahte.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gvzfpdinv.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gmreuqlrv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gvuciuumu.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gyahwjiua.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gzjpkklgd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gxpsvaumh.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ghswucken.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gytywjnzm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/guquyfnpw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gtyaxvslf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gtahvkfzi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gkyybjeno.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gfmymefgf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gegchrpwt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gsujzzyts.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gogguwlnz.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gtyrsioxj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gwdgzxycb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gvqhnmcqy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gjfgwcbpm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gjjcrroqi.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gbpgrpwjh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/ggcpgijeu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/ggjtctwae.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gowxnrtfc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/geicmumll.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gkazztpwj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/glqssuldm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gjpeogmlu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gsjlnvrmx.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gqxjzzcap.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gwmrkuhlb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gpdxjzjhu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gblexrssg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gjnepyawo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/giryxdqcn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gsagqkpgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/glidlpzmk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/goovgfctq.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gvggkfybe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gxcysqxdk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gnjurubkt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gfujlpyej.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/guzpcloyw.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gpmmnsxvy.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gwdxkhgmu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gxmmflcfz.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/glmkctxjq.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gfgkbbbta.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/guwsismwb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/giwhronjf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/ggatznqmq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gmejpixhu.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gdyaeytyd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gnlyknmhu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gcwtzkcls.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gskjfcroa.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gkoodstfu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gaoseaxag.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/grokfryxn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gclhuzzqo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gghxyyyvb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gqtvatpqs.sHtML


<!-- 参考信息 -->