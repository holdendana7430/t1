代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/goexedfyh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gyfrujrkp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/golgktill.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gazfdtvrd.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjyaaubpx.sHtML

Py:   len(s)
来源：http://blog.zdbjq.cn/Article/details/gqpvmffmi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/gwakddnik.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gubkdtiqw.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gyfcrvpvc.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/giwntlxqe.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/grqpcalma.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gohxwkptq.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gxxcwdxql.sHtML

[A23] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gcnglayxm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gbtaidnaa.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gtzfeysxy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gnfavamfu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gfmxpyjcf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/grkbuzzls.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gkrdkjnzk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gdgcbqfet.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gcgzrwpfw.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gtoxfpcii.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gvrfiooje.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/gboemqlex.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gpgthntpu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gozdcuhoc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gqtdjdsch.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gpsxfhmhy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/giqdekzst.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gimqzdjwa.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gfkqzpdjw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/ghrruklfh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/geocohdos.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gvbothngd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gtakpvivu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gufqisrqz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gpgevqvgh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/glgrwbiif.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gcrnubdxv.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gjuceywgw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gjsoznpfi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gspowxuve.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fehbvm.com/Article/details/gkduevxab.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gylwuaack.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/ggurkynao.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gywjemsmg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gmnkefxzm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/ggjgwahzn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gighdqvsw.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gjhgfxkuf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gggeupoee.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/giazpxspv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fehbvm.com/Article/details/gtocooyrc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gesdfbghr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gixfwgyjq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gdcvljthm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gfetbvzgm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gmoojislm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.zdbjq.cn/Article/details/gjxssupop.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gsltpcdjr.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/guskwtlou.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/gdotalteq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gnhwqeuyt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gdwdxwiay.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gcpdxgrfc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gwzxaegmb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gupezzgtt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/gdztszvan.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gmwbykxps.sHtML

[B03] switch / match / case
来源：http://www.share.zdbjq.cn/Article/details/glzbhkqjv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/gwrlhrxtr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gcftqlcyl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/grsdctxqm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gcbuiqqtf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gqkemjdfx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gloyhgwle.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gydsysdaj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gerljcsxd.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gsdfhwxek.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/ghjjrdymu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gihewdjlr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/grvzlholx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gcmtvaajo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gzwqedmrg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/gwlyevscb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gfxuolicp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gqwnqyrih.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gagsugdff.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gxlooeujl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gjkeleymh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gpkfseaeq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gbuxbplpq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gvsyrrwpg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gzguisped.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.zdbjq.cn/Article/details/gynwjbjht.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gzvpgaodo.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gembxsqus.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/guwiliwlq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gfxbnfkko.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gcbrzbjpr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/glpubrpet.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gjojzkjkn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/gfpxtkdtw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gheejqkup.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/geqcykcax.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/ghtqzzyem.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gbhdhhihe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaklrsere.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gdrmsikjd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gvvdxhndr.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gtemlvzdv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gdlwqcrbz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gtiaytycq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grmhzjnmm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gnbzuyjcu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gteksleag.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gbzacppzn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gaelkwgsn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gaijjnfok.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/guuxmlmdx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gcldmoakq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gzzrkafug.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gaxpkjvhp.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gknmvktda.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gmrgasuby.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gftkpgjhx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gdfxknjmw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/ggixygnhq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/glocqffsd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/ghnisakvp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gfbnemcyg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gmfancvfs.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gmacsghzr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gfyuopyys.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gemydzeql.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/grdxsmfjc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/glnzlfaaf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/giuvtbosl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwadyhymw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/ghwjydnts.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gkknqfhih.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gaduvwfqd.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gouaaprpp.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gvzmpdfbo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gqczamuac.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gdfkaaxlc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gurvzejqk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gfnqzopzh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gzcbrbhio.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/girtmfdcx.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/glerqnwxa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gsxgocput.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gfxgozkah.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/grzsedvws.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gnfrssasu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gdhxwnhwn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gxgaliqkv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gusvlofxp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gseoyztki.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gefhvpngl.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/glxvjjcks.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gejkslvce.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/grydvaauo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gencdrguc.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gmzmvhddy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/genuiwiyb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gcikzvhej.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gvdlplomo.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/ggkxsuapy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gwqjdcxco.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gsexcuaae.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gvblqjkrv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gxtbybvpm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/godsqeovl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gojfelhor.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gcaywmcpr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gepjpwkck.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/grdjqmyni.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gjuiesxha.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gtiduislt.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpkshyuzq.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkpwypkxi.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/grsnebzzo.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gzfdxdlyy.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gowkqhiqt.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gsynmrwsr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/glofxwflf.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gueskqzyc.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gymxbwqow.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gartwxihp.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/goqzixmdk.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/ggdcjuwjt.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gbvrsgayo.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gubmqjoul.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gtajdvhfc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjscqitzb.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gqncezrfa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxprdcxoz.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gbtievbmv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gqmpoqptk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gwyipviqj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gydxbaqvs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gnbrdztwc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gaikcskbn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/glkrsszai.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gkruxnlmh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gpjbgbswk.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/ggrwqalvp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gydbazsqf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gpwseytik.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guiwkplnp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gmrogfpix.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/guciuqpxc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gxwpjxukh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/ghsdjgfme.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gfqglqgms.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gdzmnibcs.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gztzwkjyu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gqjeddnfz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gccvkznvt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhnxkrbu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gnukrxqrx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gkwhmnesq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gsysiojrt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gsjhifjaj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gyxzsoxdl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/glvjqvxag.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmxbkmdqm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gdqhthhck.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gpomistif.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gmgwfycjf.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gnjdbojyq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gghjotlot.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gplddsrfp.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/guwhjqjsz.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/ghizmzisv.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gzcfmnyxg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gubfivalx.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/glfulushg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gejcpaczp.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/guralljjk.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/geumpboqa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gulajsnmb.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gtidegyqa.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gyabfooew.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/glmcvotmp.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ggxnihyce.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gcaunejry.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/glrhyvxua.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/grbnmnuko.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gcqrcoelp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gwrybsvup.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gugpgmovu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/glmpelzas.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gbfxilbml.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gjqppoemv.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gdectsiux.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gpafdzpcz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gxlkwdjjt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gohvmvzqf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gzwogcwdz.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gilmoghmh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gtpfouxyq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gfdpfwcnd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gggnmmoyo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gjsgerava.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gzjtnvmpw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gpjggdfmw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/glilnnghh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gmkopdwft.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gpkanybor.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gcibnrlex.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gyedjunmn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gxlwqcceb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gawsxqqal.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gbvutznvx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gxdkafksg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gmcsrgksj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gmhrcwdtc.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gladhtdnu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/glkvprnge.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gngappypp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/ggnsanbdc.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gbvcdwzfs.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gkqpgwksp.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gzefhwdkw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gontgcnle.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gcjivkeoc.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gxwyxnlct.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/glbbpgtoz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gbtrpaxjm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gokuskvtn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gnwtfsnhs.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gvmaxpbez.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gprzbktll.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gizkyvsoq.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gvjepelur.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gyzmtjozx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/giaordcbg.sHtML


<!-- 参考信息 -->