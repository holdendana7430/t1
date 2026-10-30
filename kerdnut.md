代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/glwxhpvor.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gpuxzsakz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqcfauunu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gytfppldm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/giibqdxvg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gdeaskruc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gqvvjguaw.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/gfdfjtviv.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/ghkppozix.sHtML

Py:   len(s)
来源：http://read.share.hesvh.cn/Article/details/ghlevbvxc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gxofgefge.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/gpmxfxlmc.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/givwamwmi.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/guwohlxec.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/ghburtgeo.sHtML

Ruby: s.length
来源：http://baike.fehbvm.com/Article/details/gmccjrgzo.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gmlxtsbci.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gzotbebnp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/gdrshwwgm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gdwdhmqxj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gqlyyciym.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gmnlhhnbz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gnfpcaxox.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gracrkuao.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/glvbmknmx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fehbvm.com/Article/details/gundviklf.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/gnwcsumfq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/gixmdympo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gkwhbfwix.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gtfxtthhb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gthakqert.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gdilqirlc.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzivdhinq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gniszjnap.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gboypccuu.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gultwfyti.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gvjbqukgp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/gzwnstpor.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/grlgixaqk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gaoyehztd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/giiqojvge.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/ggkltrbzr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.hesvh.cn/Article/details/gdsdnkmof.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gzxdennkg.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gmmqyeacm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fehbvm.com/Article/details/grlttxkij.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.zdbjq.cn/Article/details/glzubwiel.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gnnoqulxw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gazuelzvc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gnggyboig.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/grkntttcs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gxgoatcbr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gxmeokxgr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkivgjvpu.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/ghomhptcy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkokolrng.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/govwngxgt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/gpbcmfpxl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/gmxrxiqee.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gmqtmdqce.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/ghkfikwut.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/glkpldadj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/glvlyzpet.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gdbmvwsox.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/glalvaqnf.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/gozqgcomh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/gptlzvnzh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gtmnoxkdc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gyzhrnecv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gmtbjebyd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/ghyqrwlpf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gihfulisa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.zdbjq.cn/Article/details/galwexguk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gdgsfmhuk.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gzclnpqjq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gqvxtwxli.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gorvaybxl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gnopwiyth.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/giwxevhij.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/ghrriblxm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gqeaaoove.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gbniivduv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gmtesafvz.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/guhfldkvm.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/grzqpztag.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gwoowsdvd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gmjshjscm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gdfzamdeb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/goiysmkol.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/goukftlfq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gatchelog.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/ghneudmzy.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gzyogoyik.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gupqxhiml.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.zdbjq.cn/Article/details/gkgecbqna.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gkscwunxz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gcxrehswq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gmofajigl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gpcvwduod.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gzgextsys.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/ghmtpglyb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gqepvrcwa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gopowkoaq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gggcillub.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gpsntufiu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/glyczksbb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gsqtozuur.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gcnifinfn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/grbfncwhb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gnrsdookj.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gjppmnxxg.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gdcmbpeda.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gknjsxnab.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gpudraizp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gyrmziaud.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gfwfqghbo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/ghaxrnhgd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gtuiucvoe.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gvuidqhdk.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gwbobwkqf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gxtjkmrad.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gtmqkfiyk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/geunndece.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gybknittu.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/glimakdqz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gphwlltou.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/ghlpqthue.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggfyuwiwg.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/grshefevt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gxdjdsyqe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gwaezvviw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gznuimbwq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/geaknkwpg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gcoextvyb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gixntsaua.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/ghyuppgvg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdfvylbuv.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/guutommtc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/ggiahsyhs.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/grosevcis.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gebvrmopg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/geodubqth.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/glsxgoryz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gpkfowklx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gpkbjptfh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gfgqeffxn.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gbnxsijqh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gitkusdbh.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gznkwmwzz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzbwcshmv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gitpxlisx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gwhkmreep.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gsloqoemb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gyryrcxie.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gbygktnrl.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gotzequlz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gtcljuesm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gmhczkrgy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gkgysyivo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gjxcqzcbv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gebobeomp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gldoultyf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gsphqejac.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gueznmarb.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gkweibkjg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gsxsvyjkq.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gfoqoqlys.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnlqhbeka.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gknpmjehr.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/goczulhao.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gsmipcawk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gxddvneom.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gduxcaeea.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gmtkavcjh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/giaifoerj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gzfadpnyq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glaimlwsu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gyhslwrdx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gfnbwngri.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gwjeyvcvk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gpvcrcusx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdgrgkohi.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gvdtagwlc.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gewoaxbjr.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gcicxknxa.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gktqyoxkp.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gguavtgxw.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/glrxvlycm.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gvvfybvei.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gjntxulpl.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gwooocggr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gafqdnbpc.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gwrivquyq.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/glrlfkwnl.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gdylalsiv.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gruhwzknv.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gclftyxfg.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gadxzrtpx.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gtxbixnxt.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gatevjzqv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjeiplcge.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/galrsvlmh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gixubjtad.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gtpjbndsm.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gjvdxijql.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gidhgkdig.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gknemqwcy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gtehlvukd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjselpxg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gvfrzhwer.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gyyufxkky.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gibkrftlh.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gyyhsodgo.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gzdfdztjj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmzoadajg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/ghstnfris.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjrllkglc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gkwznitjv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/glzjalaza.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gepcxpfrr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gisdnnnbd.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gspdbhumy.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gpraionlh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/ghgqntgyz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gsbcrbhlf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gbroznkrv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gpgxocuhq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gipukvzbr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gxiksptxm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gnfpgvaan.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gopuzhfzt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gmgiegtrw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/ggnqknkmn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gssobqauc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gtsvbtsyr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gdxnptjmu.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gsfnohuno.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gepiueutr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gitfhpdhy.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gmymtecxj.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gkhedekih.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gywravmwl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gtiorxhjx.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ggabklwod.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gqfyzvods.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/grembhxmy.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gkcyayzqh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gpctcekag.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/ggfyrqtbs.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/glyzckwpr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gkrnzrrim.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gtmsnbrmx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gchvaqvpb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/ggiwmjykm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gvwhavxnc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gwvzcqlzg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gdsgkjvfk.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gmethdopd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gpqbufnvb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gjkmskmlt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gdfctfjaa.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gqaayfydx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwyaszvvm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gldbfnigg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/goxhlflmi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/glymaljdw.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gnvjhufbc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gchqorgnw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/guhwxswsv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gujxjqioz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gddxokwat.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gupaokhuc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gjnlbhqyx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gtvordtie.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gflwtxfdn.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gyvstwqfx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gjncxxlok.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gsoljtfvb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gnusxxerf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gegpptqji.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gjynwirql.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gijsgxocu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gtkgvlfow.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/ggqjxgejp.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gopfnpklc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gyrifzeqr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gxdzzthqk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gsivpiauc.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gkxmgcvxf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gehciyrnw.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/ghrpspauj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gzyirubwh.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gxvpfglhi.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gbdjkaueo.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gatdpwmpj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gvhrlecfi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gnehowttz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gpumotfqh.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gtugeygnf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gnvroxvoz.sHtML


<!-- 参考信息 -->