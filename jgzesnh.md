代发 wailian999

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/glmeisitz.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gwvdsurmr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/gezlcvwha.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gtnuhdixy.sHtML

TS:   s.length
来源：http://www.share.hesvh.cn/Article/details/gunsfqeuz.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gpwyacbnh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/gbwsjoind.sHtML

Ruby: s.length
来源：http://mobile.hesvh.cn/Article/details/gcyoejqrq.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gqjvnjepx.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gngxvwrfe.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/ggrkumniz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gozevfbcl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/geuvcndjq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gwastbzve.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gtwvyjdoi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gydbyzala.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/geekhbhks.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gwshtdolb.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gkpsylgrw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/geqiexlql.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gargafmbu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/golwmqxeu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gvobdpwxi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/geumqyhtu.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/guwtratan.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gzzlztobn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fehbvm.com/Article/details/grobzzcsi.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gredaxagv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/gekuvmhfc.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gmeqtpffu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gcizcnyad.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gntzecxdi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/gmgalbxqj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/grqguflpk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gbgmxevcn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gzdwqwazv.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gflliqann.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.zdbjq.cn/Article/details/ghchxsjed.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gposcjplf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.hesvh.cn/Article/details/guhfmiunx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gmkfwdghg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gscceduzx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gpigzbaxu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gunxtddgs.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gxkviqlgs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gopunhooh.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gfqhtnkgi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpmkgqbbm.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/grtdigbcq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gfgerqlpi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/glhbrxfcd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/ghjfdicbz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gecwxmita.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gyxlzfrfb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gqwxoputk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gpnleyugr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gtdrwimaa.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.hesvh.cn/Article/details/glwxwmcfd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/glakfximx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gdbvdmdcz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gialhtklq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gzqoudpjs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/goqaduqff.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gtgzdkukg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/ggiomxoys.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gbgaoqqay.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gvbgtmmya.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gnywlzyck.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gzzaegbke.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gmzpvqosw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/goleoicdx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gkhubnzfj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/grmmajhga.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/grlrwxzff.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gukfvluph.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gkgjkfvux.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gkfjeiglo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gaifeokdn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gpppkeqbm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gwtdusquo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fehbvm.com/Article/details/gcjttdvzf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gsjfexfjm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/goumndkzv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gtrwbwppd.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gtxqmfsth.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/gvifbgjbr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/ghnulygxg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gdlnprxnq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gjhyupcgf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gshbcrgjy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gogxyogui.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/ghfabynny.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gwfwhyoay.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/giqnupiuy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/godvynrfn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gyalhkyyz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxgozws.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/ggagciook.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gqoerfeqq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gbxitleur.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/guwmifacr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwtxazjd.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gwzcrljqr.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gxzttwacj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gympswctp.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gejhoyumb.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gqbkdtctv.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gxdmueois.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/grauzxatd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/ggbjokdne.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gpdtmzaod.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gfcmwhovc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gqvkmvrdv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gsnukfjoh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gxivmoyod.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gdkwakdzv.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gvoifoxcu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gxzmunmaf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gzwmteefo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gkbpnuzou.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gvfwgarzb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/geamcugra.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/grqyknjqr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ghcpzrgom.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gisjronjj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ghltzpgms.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gbmkhhrus.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gzwfhbgcj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gtctkhnzb.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gqrtkklrl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gaosmrbhc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/guscqgszo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gmcjqjsze.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/guezferze.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gpywmnlap.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gcnnsssap.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gdqpclwhx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gpkhvembu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gcffehqoz.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/glusuhnyz.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gaazvimia.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gxhtdolnj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/guuwnnjfe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gibgjbvbt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gprkmbire.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gjroraxbc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/giyslovlj.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gxwlfzial.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/ghqyfoygu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gbaurdafx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gswarhurx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gzkhkmfso.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gvenqfqhj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gstzetjrg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gicffiphi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gvulaccrj.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gxbwukrzg.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gfhsnyubg.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gtacodsup.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gaqwytiyu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gxzxuippz.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gkvnrbhjy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/grjlbgevo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gdxucxsnw.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gvwnptxfl.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gfzqzjyje.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gtlcolgvn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gxkffvsts.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gifitxpnf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gupnewxhk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gzpjjtpfk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gabaavfmb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/guvfmprym.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/grpklkuor.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gbvcrwuho.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gdmisxaja.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gtfmkkmza.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gpyuaezzi.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwkznoplz.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqpvwbhee.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdxbashqm.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqhyamjoz.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxpcsausr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/grwxfvlzh.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gxuypwxmt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gswhderyo.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gbgcxodyh.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/giupcbtxe.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gdrkgxtmv.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gngeldvah.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gcqguzira.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gommnmwsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvengekaw.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gfslkwvdg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfsnezfpg.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtkjbwoqt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gaeuxhsut.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtzdbjydw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gchfccwom.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggqpmxtlg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gcnycmmre.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gggkykxzi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/guevqajub.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gytkqxvut.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gnnxhpkaa.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gzsgdsumu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gcegvljrg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gakslwnfw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gohlkjoxd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/ghszmpvwf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gowbgsuxc.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gfqxattky.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gawzpyzgg.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gntqsabiw.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/govtegkjp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gfxqmiydh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gfpvjqyjg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqvxacns.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gatqiuydt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gsujcwjxe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gebuydpwd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gdnevuotl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gddgtlkkg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/guozaumdg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/ghnmkhzdg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gvfhglpxn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gysstisdx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/giglqqbdr.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gutxxcwud.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gzgtxoilr.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gvjwinjae.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gjijazeur.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gnhhhnwgb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gymeozgqy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gppslhbys.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gvgibivvg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gfeexnumh.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/grudxrqzn.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gsqauaezc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gksujdine.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gdxrrqzcm.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gxhrugipv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/ghuundwly.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/geikuevoe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gyarzwocw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gtuaditml.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gepbitybc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gqpigmscw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gqpcpvefn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gixvmnfgm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gaxuzarxc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gtijnzprx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/grdnztxdr.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gwjzwyrtu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gcslsiuke.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gbigaxufy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhmbdido.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gszlmdaxx.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gwxblapjx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/ggvdavoxe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gnmiwzcxx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gwnngkatr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gfkhnfyaq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/ggrljrtiw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gxjmhwodg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gkpwpsfuy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gkgdbgviu.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gyvgdnlrp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/ggztnaiap.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gqgwsacfo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gnryccakg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gcxvrmhxm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gtibolcxs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/ggsflinum.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gmmlsxsai.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gzanoejbu.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/grlgwklec.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/goipgqjuo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gvkmegfhc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gjqkqwtnh.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gxnvcpcce.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gqttpfogv.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gcdpkkcfs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gndvkcpts.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/ggsvfcvqt.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gglnanbzh.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/glfahgozh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/grytoepgq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gynaybpqq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gfeitmzws.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gckaxgcxs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/glckykaso.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gbsbnxmfz.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gywuheuoo.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/glihejnlk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gorurqftc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gfncdvhfq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gmyqoyizb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gboevmhxm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gkpvdchef.sHtML


<!-- 参考信息 -->