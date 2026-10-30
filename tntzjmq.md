代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fanxiaobao.xyz/Article/details/gsslnghnh.sHtML

Ruby: gets.chomp
来源：http://m.share.fanxiaobao.xyz/Article/details/gjricdgwo.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gcgjxrkcv.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fanxiaobao.xyz/Article/details/grilksqjz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galqxvctu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaodbjuvt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdzzwiofi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gviozbuel.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/grtwvoaoc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gftaosnax.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gynvpphky.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fanxiaobao.xyz/Article/details/gwzlvynvz.sHtML

[A22] 获取字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzopifwf.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwamyuij.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjadruqne.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fanxiaobao.xyz/Article/details/guljzmqhx.sHtML

TS:   s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gverjkyhu.sHtML

Java: s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzhofjqh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gikfaptox.sHtML

Ruby: s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gaccxelnu.sHtML

C#:   s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gexyzzzdd.sHtML

[A23] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbsjsmhxl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyfwsiyl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszpwtgqs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gzokvdbra.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gdjgrdqdl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gefnfhorb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbrapcmkm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gsulgosev.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/gihgoruwa.sHtML

[A24] 去除首尾空白
来源：http://wap.fanxiaobao.xyz/Article/details/gcbomahct.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzackmou.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyhkezee.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gbtputeuw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gppoyduwt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fanxiaobao.xyz/Article/details/gyfhmvpjq.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjieemsur.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbkxrvyr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcupmqjzo.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/goidxfnah.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fanxiaobao.xyz/Article/details/gchnbpfii.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqzcjrrou.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsamgdtzk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxyatufq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxrwjjhp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdfnwgzj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/glujfssmj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxilwjrwz.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeeuaiwu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fanxiaobao.xyz/Article/details/geeslkgnc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuhmmezo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmywgsiix.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaadezlej.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/geaorxnfg.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnszftrtp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoglchcr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gilcohcir.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggfmwomnc.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gtirevtit.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gijmoduxa.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/giqsoctsf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/grkefeifp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjefbseyg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gppzswtjp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/geqxkwujm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/giyhnxkmx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gehyaycql.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gredgybqu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/ghkntvdcs.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fanxiaobao.xyz/Article/details/gaghfqtky.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvabvyylb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyeioigb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gppdfgifs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gchjgsykw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlemgymb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkmjojyu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fanxiaobao.xyz/Article/details/ghxmjaddk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/ghbnpsplb.sHtML

[B03] switch / match / case
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxjcpmxr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpiqrprh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/genqpkjgt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlydpzpq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgnimpth.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfzyzvva.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhzbtoys.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxtjfjbs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpofechp.sHtML

[B04] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcuqarut.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyxhokqi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/glqmmhzfs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqirvrcl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuxjfcky.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvnxsnzuc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohfhhszl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkpthduu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/goofhltts.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelchntck.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fanxiaobao.xyz/Article/details/gypjyrxcc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqfgkzwv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkvpkedm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/goqgdawpw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwgponvw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gqjfirlye.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvsbfmxt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykqnhxxl.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fanxiaobao.xyz/Article/details/gliwwtrhe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmcmnned.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsivwqinu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmmpdgpwo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxradmlhy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsrqtdlok.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fanxiaobao.xyz/Article/details/gemtnqnmc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjqpvhra.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glmcjzpgm.sHtML

[B07] while 循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmytipkx.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzybbdqyn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyhliazls.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gupkicmfx.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxcvpvyrw.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcacgxcdn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gzylyikxb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gttrzbpti.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gopukxfem.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gdnrqzqjj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/gbfsesijs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gqnkqanhy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/goiidnuzk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gexqcrtam.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkshhrve.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowetylfa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/gtyahorvp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpithgffl.sHtML

[B09] break 与 continue
来源：http://m.share.fanxiaobao.xyz/Article/details/gsckaliuc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdacngfsz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfatdtgbd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiuzsgpa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gteahsnea.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbxubmkk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvfhnlzn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgbrdmms.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnsofco.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gdulzgpqz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqakbipmy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpzwxiinz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaejargv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gbazxjete.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqartessx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/glkafkajy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gocoffrya.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxejuhdv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrohgmgw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnduwxqrb.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gmsiumbib.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gavcbcwfp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/geroqcnnz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtvmddwud.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/gsycngsja.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gsdfihelt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfipuxpyp.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdaqdezz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fanxiaobao.xyz/Article/details/gasaxqdea.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fanxiaobao.xyz/Article/details/gzkzmhzxe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gywtmnbut.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcghctshy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gygjojhju.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbibdqkgb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwtokga.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fanxiaobao.xyz/Article/details/gixiosgig.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmlvuoppk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnkdwrqt.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/grafciyiz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gkldehiny.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjylajjdl.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gxijqudfl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdkodnqa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosnxxsrk.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gihsrlxgz.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqvydina.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtqydpxl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gamoqdjbc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gojdytefz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gucsjpjat.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gwnllwxoe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzljnvzc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/glsxmjhay.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwberqxvk.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gxlwlmard.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gqwjrvunu.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzybjgniz.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzmlympo.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gkggsdkva.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/glzefdknu.sHtML

Go:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gsijlyfsj.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/ggsscfhfq.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gpynlknxh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gegsuzqxw.sHtML

Py:   if not data: return
来源：http://baike.fanxiaobao.xyz/Article/details/gguysezjq.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvulmchjv.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpffabkr.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvpcxnrv.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gsrckhmjr.sHtML

Go:   if data == nil { return }
来源：http://blog.fanxiaobao.xyz/Article/details/ghuifhfuy.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzipetth.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gwxcpmqrt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxsrurord.sHtML

C. 函数与作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gkpppcovf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guwjbfwyu.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gejisvnwp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftuzmrnv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giapogyfn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpehsgtb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwlblovsu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/grbfyifbd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyunhptt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozqlirmr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpinwfpfy.sHtML

[C02] 默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gsdkmdfgk.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gyoczepft.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gntmwqslk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmxbkjwur.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gboqkwott.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/gzunaeaea.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guuxbmaab.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fanxiaobao.xyz/Article/details/gygpaqvjd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrpdszeh.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpdkybzoo.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gtuoxvirz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gamsoopgl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqghaoqfg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjgxsvbb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gadkqmqrs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/grbmsstns.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmwvlxmd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fanxiaobao.xyz/Article/details/geedbcmja.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gppdoohko.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gulwodypn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqggrwcg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpupzipf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtdjpzmx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/glifxrvjy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/giladnvxj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjvhlvkw.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwlluzxy.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gtppnlupg.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gotnoxbnn.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fanxiaobao.xyz/Article/details/ggussmobn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gggnpmdev.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gttknknbw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbruilbo.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbrwpuaq.sHtML

Ruby: return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gprrhwsth.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/glblusrmt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gunlbcsqf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gdhviwhhx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfieturac.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnxtazzy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gxhobftfe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkohqoju.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhugrgfu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gwwqfbjfu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/giyvsxreg.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gdozorrsu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojpecjav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gemldewjl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/gxcspcpht.sHtML

TS:   arr.map(String)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiscylgq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gbgvmeyyn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/gqrfvvtdl.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcszeydfi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsyfknfo.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gwauugtuq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhsatpwj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbjhpjjxd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gysppepcu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggivxohsm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhmlfzsm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbidpzxv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosraobnr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gysihoqxo.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoloouxu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlruybmr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygmrszfq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gjiteqvbn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gdwmfhvgs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gylhyxndb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfajvnzw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gihfhpomi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjaylcfx.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gfqgnujia.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gojtwyxba.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnkmepee.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmdiuqh.sHtML

TS:   同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/geifpdrrr.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gvquxbwly.sHtML

Go:   花括号块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gjomnljny.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gsnwkcrrt.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/goxfqbgcf.sHtML

[C11] 模块导入与导出
来源：http://m.share.fanxiaobao.xyz/Article/details/grizgdljl.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmfhjzpl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fanxiaobao.xyz/Article/details/geddxtjss.sHtML


<!-- 参考信息 -->