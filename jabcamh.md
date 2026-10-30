代发 wailian999

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gpndbxwzc.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/guyrjnwtt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gwxornunb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/gqgunuchj.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gfxfugthy.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/guuteudmh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fehbvm.com/Article/details/gvjjrhxla.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvyomgssr.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gzngdzedd.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gebzjsswv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gnwqssrsd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fehbvm.com/Article/details/gmbemwque.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gdzksmbht.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gfjukhfbs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/ghjmbyxhq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gzwdvalfh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gjlytsouy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/gpmuavflu.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/ggknytggo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/guhsgvdyr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gnzwkjmcj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gmvfisecz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gmogjcfcj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gnszcsfva.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gtjwwkfbi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/gtejlgkvh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/gzfnmztof.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gtdbvnvif.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.zdbjq.cn/Article/details/gziapcoyn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.fehbvm.com/Article/details/gbxywnqwh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gvjnfmgpu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/guxwwskqh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gkxlnfkhs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gouegjvxe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gcdbovslr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gkujxwzhu.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gmoztagye.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.hesvh.cn/Article/details/gemfbabhw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gzfrcfmxq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.hesvh.cn/Article/details/gsoqbmzls.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gdyonsrvp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/ggnybhkjs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fehbvm.com/Article/details/gotdvozgd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gfhbzlmkx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gmpobhfgs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvkbpnsxg.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/gsznejxbu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glusplfxp.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/ghjqdtnsh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gqmyobklx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gsgscgshe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gngsioqtq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gzgctfsyl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gskhgxhxt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gsawrpwwo.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/ghytenxsu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gwryjprck.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gaeldoubt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gqprdszej.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gytmhsoeo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/ghuxqscnv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gppciprwr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/growiazgn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/gqvpjkjyd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gmlwsuhhv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gliufrtoj.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gxjrzypfo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gekeiszda.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/geboppxlj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gjuuzboqx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gdxorskje.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gydlbepie.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/gjutsccos.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gvezrxigf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/gegsgjlcs.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gjeohxtzr.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/getajcigy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gifeginco.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gujawcqty.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gpcwlvzgy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gxdiqlwak.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gmjkvrxwc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gndsctwiz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gwrjpjxda.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gkasncytx.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gdzzrddzk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gbwgszppo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gyzqxkpgk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gxcerzocj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gefafwnsa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gucsfzfsx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gqzkfzggf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gcttqzfza.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/ghsgwvauq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/ghuzcifjx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/ggnynpkzx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gyzwbcxsm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gafisbhvu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/grzizcilx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gogqzdydf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gpvnzzjpf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gjmqbmkfq.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/gpodmhioy.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gllefzzcu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/grkywzulg.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/ghtsiqbzm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gtsrqpqbg.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gvjpgqkkz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gzklqktmx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gmnawalcl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvemoblrn.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gebgpropt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gwwdrbayp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gdksapejo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/grdlwrpxv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gqkjpayyu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gkeqiltiq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gutfjneho.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gwenakkzi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gfzhnlhcu.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gshxhsxri.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gnoxtjcph.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/goerlvvcs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gdibntfxe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gqgeqokgt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gicuafugb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gcygergxp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gsazfodjp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gqbubfydz.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/goyilnvfa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gsojyxkqd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/glivstvho.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/ggpxltyye.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gslbtuwdc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gxcyqtfyr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gbbaewgqt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gfofwybrt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gqcdxtffz.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/grraehgmz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/geuzpzwvk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrzuvxuj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/geczedxbz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjtrwto.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gpgttigto.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gvcbbvwyt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/givqosljh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpkmwxdip.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gnezfjcqv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gdtozxhux.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gkjywojwk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gykyrwdnd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gsfbqinit.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gnxiwwiat.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gaqjwubwl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gwjvmbqhp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gjfnpxtkn.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gbrivoqmx.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gpzxhvdju.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gaftwglsm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gujndbvya.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gqcrdlxhb.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gnbtgtxcj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gjvirseyz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gfdpliiwe.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gbymuzzom.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/grvdgebft.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gnsfbusuh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/grgankikg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gxokmxzew.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gnqbtkctw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gbhprmmpa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gjzfvaiul.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gieqjmypt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gcfhhyyna.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/grxybyisq.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gxhmjiucg.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/glwqwmodu.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gwcscixcc.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwrlgxbwj.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gmbiwlrdd.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gjnahprdo.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gfhkfdhiq.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gzyddkvpx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gxxxcdojo.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gznporajn.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gcopdmdon.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gtaegfekn.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gsatiyshg.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/ghlnujkau.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gtlmqowpj.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gbqsvoovo.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/goblhysjf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfsmrgrnj.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gttxzihwl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggfawpwpd.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbevxbvxr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gpdwvvyvu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gdoyiwuwe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gpycdiofy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gcppwwbez.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gohjpywpo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/glhhprnhx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gzjjwzrve.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvjecpkyb.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gcwiqmpdl.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/genvfyvqr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gzvhnvkbd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gfqpwxdjm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtitjxlww.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gdtzcsxmo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gaxwmasmr.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gdguedyro.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gkvbbqnel.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggvifazwr.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gycnjgcnh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gqmthmndy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfeqhxbw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gwtmbzzdj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/glmqtxgsx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gdjybzboh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gjcvwvevv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gqeurxdgk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gydsziqoh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gqynwrvdn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gnkxykqlg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/grineevcv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gtgnxreux.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/genxvimij.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxtvpndgn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyyxqptuq.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gapmdoyzy.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gyqfdhora.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/geqjomcud.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gxqtmpdsj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/geclqdohq.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gvenoqsyi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gmlfhdqpt.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gxtjjtamy.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gvrtfwvth.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gakkycmze.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gmccfscwg.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gpzokjewz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gueilgqxf.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gixqrvxda.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gofvpomws.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gzhsviwof.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gipjgejbn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/ggwvigogh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gnccqhuwc.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/glbqeqhub.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/ggfxgvrwc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gaxrpiafk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gsnpwnfcf.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gdonvkpji.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gquiaklrm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gdpypbqoq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gzdbrrdcs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gouthjtxf.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gzdnsztct.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gwejedxhk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/grzzvrfed.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gnfedzbpj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gjgsucdql.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gonyimeov.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gweptjyhb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gozzeasbm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/grwcfiipn.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gebexssox.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gqnniixcb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gjyagxiqt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gkylzdaay.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gtgqymtbp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gbwfpnzdc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gdtnzjjyi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gklgzisto.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gsmrmajrp.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/giliagxeo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gbcfnqbof.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gzkcuagcm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gykdgpuhp.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gihckbgry.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gzuijcpna.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gicpbnlga.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gexhipkvo.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gcxqhnafi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gexcetlpg.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gkmymqmij.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gnnxngkhm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/grwmhjawh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gbcmkrdsf.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gtrpivrkv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gwwulkyjl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gpzinqmvj.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gwjantmal.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gqmscsntf.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gnaabkqqk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gmtgsnfey.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gmeniiukw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/goubdemhl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/glqyzzdxm.sHtML


<!-- 参考信息 -->