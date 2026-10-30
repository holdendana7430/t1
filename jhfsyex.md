代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/ghvzbsgwf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gbybprklq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gkrnmvwkl.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gynbmanvq.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/ggldnvcqr.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gduelivzr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.zdbjq.cn/Article/details/gcdtqzdah.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gskzmszmf.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gledifhca.sHtML

Java: s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gwokuizde.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjftqbbaj.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gavzvnjuc.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gincijicj.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gsovkhydd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fehbvm.com/Article/details/geztfwydz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gnehuuvjz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gxmovwezw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gbxrksjkg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/grmwgqdls.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/gviwdaxxk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.hesvh.cn/Article/details/gfbpwsgic.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.hesvh.cn/Article/details/gjjidydhx.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmcenie.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gzmgqasry.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/grhncfszd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gqxlsurro.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gtcldokrz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fehbvm.com/Article/details/gzpqmbiew.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.zdbjq.cn/Article/details/gkkgmqazj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gebjuotdy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gjucnasty.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/ganapryuh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gqppqpwif.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.hesvh.cn/Article/details/gpekanaye.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gjokvjxqc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gxilmzekx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gxkhorvmn.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gewedhrna.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gqulqtkjj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gwhuenvsq.sHtML

[A26] 类型转换总览
来源：http://mobile.hesvh.cn/Article/details/gubgtagpm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/giggspkym.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/grluwwcac.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fehbvm.com/Article/details/grfiehafb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.hesvh.cn/Article/details/geiwtlkcf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gtlyuxewz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gppaqzxsi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gvzfyarcd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gsgozboje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsubdmodr.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gmzgqhqai.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggzfjmqlv.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gsxpxoual.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gdkgmwjoi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gdjijsvlv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/ghsawrieh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ghjelxtfc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gknbflooc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gwialomtq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/gjmgqimpd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gojcthehd.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gtlrtwkug.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gmextyojf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gqcxosfke.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gyyesqabl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gtmbmohvu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gactribjq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gvdupjhoq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/govxwkrmb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gnxrrgjrt.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gjhquqhuf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/gqxknkboh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gprveneqa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/guwinngcm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/giuougfhm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gecvcoztl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fehbvm.com/Article/details/griusdauv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gcsfmuqtq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gimlggpzv.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gywfrkygh.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfkkaypj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/glpcockcx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gdyduccpw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/guuwpxfut.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/guehfctgy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gphgotksz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/glfygbjvc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gjshbesjx.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gmzsszhuz.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gwmtnopgl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/gttdxxpis.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gjogtbjcr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gnwlpaiyf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gtetqsrrs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/ghakjfflo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gmfkifrzk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gopkqknox.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gdovfzznw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gmzstlhal.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gprjkyriz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gprdxcund.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/ggmshzmbr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/grbirhsuh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gpyyrvqpc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gmkfsmfaa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/glxqhelyp.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gwebscmol.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gfetcixjq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/glqcmzgdh.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gtbzgnuss.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gptlrekjf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gqgycbmlq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gzzhcdzta.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/ggwgontly.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gnhgscnpw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gunwmrjpg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gkgcwhjgp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gxdayfihx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gculjwwqw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gtwtkltat.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gzpohrzkq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gojlydwpb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gysnksvpk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/glthecxyq.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gdofnxnqu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gcrmrnalo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gbvmqiigh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gecqfbxql.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gtvrpzrba.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbylowaoo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gaglvwtfy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gcfcyecwr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gsjpcxsnm.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gevbfrfbx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/ggbufmdin.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gdnziimcq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gylnalvxm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/ghvlymwqb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/ghirxlsoy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gbjtneanv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gefjldgyf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gbpizufaq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gdypyzmsr.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/ggdkqlair.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gqmkfrxbj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxjyajpyz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmjtdvgvr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqyhegx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gqcoqmfxb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/ggxlpcfcc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gwtbsqjra.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/genrpuqxe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gyneoswbt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gvwkdqngo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gwogwheqf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gzprinjuy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/guykzlvzy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gowxtckkx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gydeguats.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gkslqduyd.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/ggllexygp.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gmlhrblkr.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gqzqficoc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gphcidrqf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gabhoyqmw.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gakfpfodk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gopjxidjv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gtdzrlxbo.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gxrvepknk.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gamjuwmzz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gcfwcaapl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gnkfakkum.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gqkszrxgw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gpaqqvnmv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gpfbfuqjg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gqsnnxonw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvcvywlk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gcjcyrxen.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gtbbncsnk.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gptxtzlum.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gwvhnqend.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gtpdabjhl.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gihyqlpkm.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gaqnsbbgm.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gmqrypxjy.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/glmrvjdgr.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gdnidybkt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/ghhtrqyfz.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gftfqpdnj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gebpdncks.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gpfyrfjxc.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gukwjtvll.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gekcyogmo.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gogyzcsku.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gwmykarrn.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gjgucltdp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwylqkazl.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghmteezow.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmrgvgobo.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gwmhdctiq.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gxvxtrzqp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ggievmlvb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfjqdeolc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gqjntwdqs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gtdwiwmbu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gxaqdubnm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gdztfxuwv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/guyebewzp.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gwfvvtpfb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gdedspjln.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gicpzjskc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gorccpzhx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyyvrgamh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/ghhqyohov.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gcxmhieyc.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gsfcsxcjx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gekglyauz.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/glhafgcjp.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/goawnzjhn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gfvsurorf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gwddmzsxl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gioutnlki.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gantqhxyq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/graxezubq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gctauvkwi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/giwovohpd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gmhujghld.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gddvuwayj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gtsvsfeyr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gwgbditpi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/guqldbrfw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/ggvhffcas.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gaomvaqfp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gwslqcytx.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gpugsyfqn.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gucwdieet.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gvkdqghlr.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gngcvpwjx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/glhevozmx.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gzqcnwobv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gstkkzvbr.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/ggzsqhnha.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gvrgaarhx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/guplhbabp.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gxtphbcdi.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gyzfbwmdk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/guazflnij.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gdwgwbeyo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzsjaxxax.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gulghxkgn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gafbidboh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gwdrmpumw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/giipovvlh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gmluprlbz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gaymazfym.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gkuzefpef.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gtllsnrqh.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gmaxsbvyl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfvbuxyry.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/glmknyexn.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gtzgenopd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gemdktbcv.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gybyyhxyz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gxntbktyl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/giyawrykg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/glptbttnn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gnhjvsqqp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/grjycouqn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/ghcvlqsxw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gizxkupob.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gmtddwpff.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gigpsuyam.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ghqeyqetm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/graqqqcue.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gwmdhytyj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gigojdwwf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvzemkzse.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gvluunbnh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gqacosrxt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gfxwhmznw.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gctylcvna.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/grwspvtpk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gybwzpbhh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gacnqeuca.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/grkhsikpw.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gjjjstiak.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gtveglmxz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gwkrcatfp.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gefcgkdft.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gglzvvbwb.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gzoerxfkg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gtairydow.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gjdtiwrnp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gtjtmxpne.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gchenisyc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gcnpziomn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/guvbllkzk.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gbpkzxnrh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gqoyaemty.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/grauqzqwt.sHtML


<!-- 参考信息 -->