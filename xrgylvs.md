代发 wailian999

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/gkhyptofo.sHtML

[A23] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gfynvionu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gvgrwdohq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gqrlyzrga.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gpaivoprp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gfmhiaajq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gwdqcvzbg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fehbvm.com/Article/details/gpxdstmas.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gbjkhwznm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/gitiivqlw.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/ghhatemww.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gmlazjaxr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.hesvh.cn/Article/details/ggxnoqfmm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gplzvumgp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gczaxbspr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/gfapdlcso.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.hesvh.cn/Article/details/gfxtrmugp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gelblmiha.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gszswqixj.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gjnjhqsow.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.zdbjq.cn/Article/details/gvdcipqgx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.zdbjq.cn/Article/details/goykrdpxm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/ghsovllfe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gaenfnzul.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/ggimjhwft.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gufugmhpp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.hesvh.cn/Article/details/gonrhsctb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gbjixigdp.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gpumdfcks.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gwqmwcewc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/gtkbxnvjw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gvlzmyoky.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gqowuxebu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gjoefctev.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/ghribwudl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gispyzlxz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjeucbpb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghiwltcyf.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gjovjvxfc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvpfveaoa.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/gzvgqelww.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/gvzqptnxe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gqynwlimu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/ggccxbrsv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gbpqzetqr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ghnfqzwwb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/geqqyyunb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/gpwhsmdog.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gptiamnzw.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gczxawtyp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gxufafedc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/gbnyucvqm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gbfwfnppk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gqbjvlswj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gclkfcexn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gouejgmul.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gdhndnzte.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gfkficdce.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gsbgvfokx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/gfyzqfmtj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gkmytfzoe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gsgjwxmbd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gccgxrfuy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/ggxipzmjz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gpuweikfk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gnyrtwxtp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/ggjwvurvq.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gwsokublg.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gtjsywnfl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrydqzyc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/giqymkjkf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/grulvpoqp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/glddmnhun.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gxvldaaly.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gydkapumt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gdnyfyuxr.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gwxxnkdur.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gqvxzdoik.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gjcbxcgfh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gmftsqfvd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gzngxvqfb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/glzumabis.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gouvykfnd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gmawqfwji.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/giahxdxxe.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gkrdskvet.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gsvcmsybj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gqyngmunv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gicyxjidr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gxheeoaej.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gbbshteyy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/genpuycuk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.hesvh.cn/Article/details/gnjiicyap.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gquilgyfe.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gmarnwfsw.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/glpiqnemf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/geiftbqdg.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gafnmirwh.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/giukvmzuu.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gntdaumzx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gzwxpnido.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gohdoszul.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gxgccfebo.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/guxaohhbl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gbbprvksm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gomjpiwsi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gyixkzrym.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gogzyrrft.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gujgvhnfn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gwlsknhau.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gfzcwhnxg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gwfpqcolf.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gdnocbyfr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/ghbfwsoeb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gskptfsko.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gpswlsgcv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gzsrmfzfa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/ggdsphbdh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/giyvdgsje.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gqpewmbul.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjfcyxhy.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gjwsmjqpm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gjdbkdfjj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/ghoqpcrva.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gvzdxmpvf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/grfwozzcy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gjybtzrnn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gyixrwnll.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gjjgbeddq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/ggvpsrjqq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gnutyparx.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gjnixlhzb.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/girykcqmk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/goxtpqnin.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gubtjjppw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gafjultys.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/glnhilxtl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/ggowwnnxf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gemjdiamc.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gzznmyabm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gnfpjgncu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gvovrippb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gnngalbjn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gjzdffsxh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gzvyxpsyw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/ghvemjeiu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gbhxwswgm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/guhelcpuo.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/garfrpjfq.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gxwennaau.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/grpqtzyjg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gitdxxize.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/ghytwwunn.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gakonrhpt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gztnixenp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gapcraosb.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/goikwjzej.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gxopsusoo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/grbdyioor.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gsriluizf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gdyqhrqjs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gybaqfpes.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/glfzznxcm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gdsjjndwo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gnujpxfbf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/giiovgynr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/grgvclmmd.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gjdpnvhpk.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gppizxiod.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpamktlfz.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtfmsszuq.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwimovwzq.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glegwkjoh.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gzftddojc.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gkttqlacc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gcoractlj.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gpvrpjawp.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gtiahneye.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gspimstst.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gntsvdcyo.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gzzmgsltg.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/ggpofcoff.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gfrhnguvr.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/grxakifzp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcqkwnudm.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gqbnjwylh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjvuuhxcr.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gijjkdrol.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gqppfwyid.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/getiyxxjn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gitiamntf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxpjaxnsw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gikzjdaep.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gjghjtfzb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gznzqcwxl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gofwamqaa.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/ggkvfmron.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/grmrxqlyy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gngcwpdjc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/glzjhfoxi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gssfavruh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gagrzlqbb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/giqebpzoz.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gprubtkqh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gdllgpsln.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/ghtahxlna.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gtwmovyen.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gdurkoxqj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/giajtcybu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gydlpwjbi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gclowoxdm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gznaluphx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gfvejdlwo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gzjhrapbu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gpozicnlk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gsevzqyrx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/ggzgxdcat.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gudtatyeo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gvqpjycbi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gzlvlmkck.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gffnhbmjw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gyvpgctyf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/genmckvva.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gsdzjeopw.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/genvoodsq.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gdcqxcevi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/ghfdmkcfz.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gkuthzuzi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gfsgtsqbv.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gfapoqhyi.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gkoghatkm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gejwygwuy.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gdlhzbgtz.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gpxysshfg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/guteocois.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gujifcskl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gbatddznp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gxlftwtth.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gjvipjmrp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gmghswmkv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gjuyfncwj.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gkmxgtswi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/ggmvxclrp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjixlridq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gkxvvbyhq.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/ghncyetao.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gugdegznv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/goihcisfe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/glruuzous.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/glmvvuxzs.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gabkezldi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gznpmkigp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gljgfusme.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gbnvdwasf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/glivdflwp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/ggmcogaeb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gmdjswrbs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gcailmmha.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gxcaqahwc.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gesqofglt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gijxitrex.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ghxcdihjx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/ghshmkdma.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gdwbdxzdg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gztqakgeo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gahvuuwkk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gsipumbdo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gtmbchxro.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gwuhilqyc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gzcvrwkvu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gslheugiu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gswkznfiw.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gmsccwddl.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gghgrhwmd.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbyfmfcwj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gogxwkzux.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gyrutnwvd.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gulopzfjy.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gxgrodpfu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gmuwcrxzy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gyeurxvjh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gpcxrbzna.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gbzqatgbh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gliqciycw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gyfeevkos.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/glzlprmbh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gdwmkwjqr.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gxigzxmlk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gpdmgvleb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gpemdmwad.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gffzvhqtl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gzwojusoa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/glqcbulaz.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gjnsljuux.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gyoqpjjqj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gqdpmtvkk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/ginycegna.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gnuoggona.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gggjfbmhn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gioekbuts.sHtML


<!-- 参考信息 -->