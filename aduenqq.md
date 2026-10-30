代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsfhqhuo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbxodfki.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxzqxpyzh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/grvdmvjdj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gvsetngtx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjncnlqbc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/ggtxwydsx.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsiavaws.sHtML

[A22] 获取字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqepbazme.sHtML

Py:   len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzqazzax.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fanxiaobao.xyz/Article/details/gishybban.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fanxiaobao.xyz/Article/details/gexaqnqzi.sHtML

TS:   s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gzerlddsp.sHtML

Java: s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gpglhvwhr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghswpwqlw.sHtML

Ruby: s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyiibwke.sHtML

C#:   s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpauqekm.sHtML

[A23] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdwfyvzy.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsulhnsfe.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gevxojvhl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gsnqdvnro.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmolgequk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/ghgwxuait.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqcjdcpoe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/givpdwdqx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcvzrwmd.sHtML

[A24] 去除首尾空白
来源：http://www.share.fanxiaobao.xyz/Article/details/geojdqlzi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsugbkqn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcrfichwt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gujdmcwnw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/glvgikybz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fanxiaobao.xyz/Article/details/gteunvhcw.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fanxiaobao.xyz/Article/details/glbvobecd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fanxiaobao.xyz/Article/details/gnhrwpksu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gmedskvyu.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjkxpblu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogozvsub.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/giaxblqsh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/guhombbwr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvglvhbrq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gddcgwmzs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhuxegdt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvhkzjbf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gembuqslg.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/gxrgkdbpx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdasbadve.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkvsxtsy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grexpdjjr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fanxiaobao.xyz/Article/details/gvsabhkmx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/gznvfayvs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyflysyix.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gwojpbhft.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gyvrycgng.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnotllyk.sHtML

B. 流程控制
来源：http://blog.fanxiaobao.xyz/Article/details/gmjayxcbp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gedtepieu.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fanxiaobao.xyz/Article/details/gljkodzuw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gukfxffiy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzhhtbnam.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/grkffycex.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gakdutwsc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gxoggwovs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipbuefod.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaaxdqch.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzloweob.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavvxilyq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqadooz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvboromto.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzyteatk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutjjipde.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/geuwytsxn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvmlqwna.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjvytdtd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjslhgsmv.sHtML

[B03] switch / match / case
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigtnhyus.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fanxiaobao.xyz/Article/details/gzwwkjfqd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gatsskaav.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gehreiwjp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glfbqxwwh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ganwpxgkf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlkiwntk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fanxiaobao.xyz/Article/details/goesxfulx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gdairivvn.sHtML

[B04] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmiecpdr.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gayfbxvqz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwwaadgp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvkdhqud.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqevcsztd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlservez.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/gngweqsil.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkobbruar.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpbbvvyn.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/givvwpmjj.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fanxiaobao.xyz/Article/details/gqirjguyg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzhaaokde.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gecfguesw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnddoldvz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnnhiicq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gelndqftj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjpnzvew.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtoamfuo.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfiuuvro.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqazdrff.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gstazvdix.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqrgkqky.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfchqigc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goszlkmiy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrjcdpqz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/glzqfcxoa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdwhriqgt.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfxvzxzn.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grviwrpmk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvynsobkv.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfdjrfyeh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkjtcfun.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntecflsu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fanxiaobao.xyz/Article/details/geagxqgcb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjciootxb.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyinwswlm.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/grjyalfnx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fanxiaobao.xyz/Article/details/gxrqcmpiu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gxmspmuqo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goudahxrw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjnuyzkh.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gcdmjstjh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/glzspfljh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxprjksin.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqoxlqne.sHtML

[B09] break 与 continue
来源：http://wap.fanxiaobao.xyz/Article/details/gvtcchzev.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfpruwwm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwasgwhku.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaymshpog.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggttzrplv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatgccnnl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkdiwgxm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxxdlxso.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzbnhgvb.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gyxjticfz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fanxiaobao.xyz/Article/details/gtldhjqba.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gallutoef.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrlbyrco.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gomyqikxa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gimlbrdjw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gchbuiuuu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/greeufedq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbklydbaa.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnpnrnjw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtisyhlqk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuibnyma.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/guhrhjkyi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuiktyxv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxbsqqbi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/glnkfmycz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmtuetej.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmfnpoau.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghokselsw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffysduwr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/gjwymtbjz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geghgbvfp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gknfdazkf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gyxlspzif.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutbmqruh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuimcyjh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gwcqwvbqh.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtiqdhfmf.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/gxoxhvfcm.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutlatikb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gpxsrkffh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gryqmeqym.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gwtvnybpf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/gcijqfqte.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfhpahsa.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gacgnfykb.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gggvyhdma.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvpqrdva.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdijpbvx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gssyivllf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gxpozddau.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpycmpgsd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfegemgea.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejdsocie.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwebrjane.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbbpnjnx.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gyeugvled.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fanxiaobao.xyz/Article/details/gawwqjtxh.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gjzkqehkb.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/geljqukmg.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuhfjwmc.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gqokwqfjr.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gvarvspjd.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvkormhs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grypynxsn.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gdffkfacn.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlmskffq.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljcchovc.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsklcdwo.sHtML

Java: if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjmxhzmb.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbaewgoq.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gshszelau.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gxayamawr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwadpyfy.sHtML

C. 函数与作用域
来源：http://baike.fanxiaobao.xyz/Article/details/geujjcroj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdavcfwt.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gulazmpvs.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gvyvavqec.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwwpixrcl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gozqczsgj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqpifzdl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjyuqjzs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvmukvrf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjulkudjg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvtaykne.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaumxter.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fanxiaobao.xyz/Article/details/geiiwtchn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdoqwnmz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsxebdzi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzrcgvxy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/ghrqkjzoq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlllyzrd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbqybchp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/gzjbazokz.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjasqeazu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaaaxymh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gumyimgiu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gaybegtxy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmrvtobxm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqipemjwi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqvdxghq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gesxqdikq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/glznvjwgy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gyznncpkr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gvlmnotjv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhppzanw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/glhkzuios.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/grkwerrmh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/gnaukpvmk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjzgobgu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/glycxdpcx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgcdmrvu.sHtML

[C05] 返回多个值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmheoqtp.sHtML

Py:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvebkqabo.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgvdusqn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogxczpyo.sHtML

TS:   return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvdrjnwd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fanxiaobao.xyz/Article/details/ghujijghe.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/glclfyzgb.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gdrrvzbox.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkzqtsr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gcaabyxgy.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyfmuuxn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/glnftztfq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfrmqcr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweotbnov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gxdlzranf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gkwqyosdj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginvqkxgw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gexfmegxj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozcspmvl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gpyymgyxw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/glyysybcs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/gtpxzablj.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gganrlvbw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvosqklb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gciothaep.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvbzkyod.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrdkabcm.sHtML

[C08] 闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gqtwyuujf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/gewtiunli.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfydqrkh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbacjbhyb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfldbrldc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxbqnasd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbtykxil.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqkijrpk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/galbtemwa.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gowhtnsov.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfvcpydsf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gakpiqylu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnwhfahw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gekpjbnvb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghmdvrmsu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gggicqcqu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/grizuqjya.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gieyumzeq.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gugeemaoq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fanxiaobao.xyz/Article/details/gncrltvrt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyysbind.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gmspzwvug.sHtML

TS:   同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggewfnqam.sHtML

Java: 方法内为块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gwdhyyygt.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpxdzsrf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaelhfzq.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/goywlnjip.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmnjhkts.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/gehqvdmgi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrxwzvky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgxpzavm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/grdqfnvod.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/gmsokuxuv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtduhnclb.sHtML


<!-- 参考信息 -->