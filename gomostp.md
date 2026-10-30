代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gdvpizyaq.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gnvyrmlrm.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/giazawdtr.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gcvuqjool.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/gygcgyair.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gjdurldwf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gthmbwqso.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gpxtfucle.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gdoiltdqv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gyfvlhzbf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gmffrndzw.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fehbvm.com/Article/details/groigixvr.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfnihebud.sHtML

Py:   len(s)
来源：http://www.blog.zdbjq.cn/Article/details/grlxpehnn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gpcctgdqy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/gsorluacs.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxpshnc.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/govoxxfvd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnviadmx.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gozrsxqnd.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/geoakgmgm.sHtML

[A23] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gbizvgxco.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.hesvh.cn/Article/details/gwyvbfkep.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/gwxrqpeqh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gvcjostrh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gyupspycb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gemlrqkkw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gsnzcvxpc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.zdbjq.cn/Article/details/glkzbtsml.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.zdbjq.cn/Article/details/gzpnekgyl.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/gsztbsenn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/grfuoeyhy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.hesvh.cn/Article/details/gjmhidybb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gqkesryet.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gzagudmyn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.hesvh.cn/Article/details/gbneprwhm.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.hesvh.cn/Article/details/gtnqwsupq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.hesvh.cn/Article/details/gzvghgqhv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/gliuqnvqd.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/grfywgyzf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/ghqiyibgs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/grfhmicmi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/gecmwjocu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gltunfost.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/ghrfwkabw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gfydpsmxj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.hesvh.cn/Article/details/gsvnuzldq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gtezqpbys.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gowxqzrql.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.hesvh.cn/Article/details/gfdogyihq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gwcakjyhl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gjfwzghjt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gzthtdhhm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gsibdjsry.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gupxpanuz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gbcqegqmd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/goxzsagdu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmparkdwl.sHtML

B. 流程控制
来源：http://mobile.zdbjq.cn/Article/details/gzatorqzo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyutoydlq.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gsfolqcog.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gpevrnwid.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gyutgraap.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/ggkozqonx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gcytwbvwy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gnrpteora.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/gowgcdiyx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gbpokckjz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gmpbeyzdy.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gcfveecfh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gxzfhfyqk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fehbvm.com/Article/details/gqsznfhqv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gznkhppxb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gyubcxxmd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/ggnesbdkp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gmlxesfwl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/ggqfwgpon.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gldudwqrh.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gbxgrkzwq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gljpkvaho.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gsjxuouhi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghqmbbpwj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gryqgsuky.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/ggexqbcib.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gopmuykby.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/glfwxmvkm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gbybiidta.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gpyhkrkyy.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/ghzszpffg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/grbgysdow.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/grvekkbpn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gbsztukis.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gcsagjrtz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gpglxabyv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gicshsudp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gdlkkzahk.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gylrjwiqe.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gwzeipikq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gsbtenvsa.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gyapahgsb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gjdgximyi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/ghhpxkwym.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gavwzqtua.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gqunbywqg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gdqkskwze.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/griejhtwp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/glzdkxvmo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gfvpwrqiz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gggfjajfl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/glqgwwfzn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gsaroazgp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/ggqrnigey.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gazgeadll.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gcxoxbeht.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gwnjjcfey.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/grbkeyrcu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gccrpgtcw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gqpfanzxm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gzgftoufj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/glhbcyxzc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gvzelrjcl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gutosvrbz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/guidvvqvp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gutlczjat.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/ggmdxebsj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fehbvm.com/Article/details/gjqchdqoy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfeylrby.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gjygwdxlp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gcwmdkmcn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gytheiclv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gvtkzqirq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gmbemddzt.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gpehzampf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gxzjynhuo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gmlyqcasv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gpllykbgs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gxpypkqmp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gmtifzdyy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gbrzzhevo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/ggcjhtqfr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gkxjhqrbg.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gopnvsevz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gzjewribg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/ggaccfnvh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gssqidvuk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gtvfvdsjj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfasvuuln.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/giaoblipq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/ghcvgayqw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gmigzyibs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/ggfbhnbbm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gtcixejrx.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/grfxmyvug.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gplnvtofn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gotzmtnei.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/ghmzjitdk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/ggfngoney.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gzrvagizs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/ggtsrxfaz.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gmcfkroqd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gtkbseemc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gkjntkpcw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gdsuxjdcf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gyfskskwp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gkdunymwc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/gtwaribbr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/grcrfjkan.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gftikojij.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gomehwswm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gwylqdmgs.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gfbjeffca.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gnfkubxdm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gbniwtptg.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gvcprmtec.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gjfljcrws.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gvtjmgirh.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/grgmktlhc.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/ggwnbaqdr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gpvdnbpko.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gkysugrhw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ghgtnbilr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqbogbxcz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/ghuumhwxx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfukrmrbu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcqmqzgp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gqomuywer.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/ghewbrboe.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gpzzpavgn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gdkweiytc.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/grzwgvyhu.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glkcnixhc.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gakculowk.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/guzlmlxzu.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gtpnpwsmc.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/goluycpah.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gvsolustg.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/ggykpafve.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/goifgelpk.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gxsnjuknv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gsgtxnuih.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gfcmnnrbo.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gxnjyndaa.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gkqspuegi.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/grrjinsgp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvjglppfs.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/guxzepckc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gznvegyex.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gnmjhfanl.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gtwabkfrd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gchfhetco.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gotunvuec.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gmqjqefzo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gqzyxukaf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gwnchsguf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gfhfilowj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwcjnspt.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gopobibir.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gasxsiwsp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gxxtdmiyu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvnahosin.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gikaqcahd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gpqyeeugs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gpfbdnkkr.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gcygommdv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/guejdzgcr.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/grmlxuegq.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gsrvyzbuk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gqlwsdmad.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhdjokay.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gwndsfwbj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gguafilid.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gdhrjvxga.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gxdedraxs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gbweotuat.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gwjhdpsur.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gksmlusva.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/ghyhaitgz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gnsvadycj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gjxjacsur.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gicnhxxtd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/ginazenvr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gfzohvdmr.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gtrwifhrg.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gurdjwkdj.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gqyysmaqe.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gvgycgfri.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gneveetne.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ggbfgbmvm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gjjsbsbcm.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gmubgdkbz.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gtstrpimq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gcoxfnelz.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gcbdonpzw.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gzedtrljz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gpjqciqra.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gtmrrgyqe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gcimbulvh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gxdghphwv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gjpyswuyf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/grdhwqldq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gvvyskfcf.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/ggemppcch.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gtsliiyaq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gvhvxgzhr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gggrzldjl.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gxjqqwpnr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gfnuxnehn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gnshlgnyj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/goqcycqbd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gtcpfyvqk.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gxrfehgim.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gylptzylq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/guuumtbre.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/guwjybxam.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gcmlitdmw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/glaojklap.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/guemcbedc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gxdbcqykd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gcctgipcp.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/ghkkmancn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/glvibmhkm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gaabepjmv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gcfzopnyi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gjtahebon.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/grgaqzplj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gwwpzmzzj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfiafkius.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gfozirjmx.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gjozwdlbv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gzjwoqwsc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gqupkufuz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqacfauwi.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gvyojsped.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gyvwmojez.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghvkfxudp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/geikfbmpu.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/ganhryldt.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/glguqmciy.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gfygyhtrp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gzvprzhht.sHtML


<!-- 参考信息 -->