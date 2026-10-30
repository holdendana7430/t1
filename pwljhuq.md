代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fehbvm.com/Article/details/gsqyrkeax.sHtML

Ruby: gets.chomp
来源：http://wap.fehbvm.com/Article/details/ghmzbuamd.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gvveknaee.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/gxnsdbtim.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gggxdynsu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gybtutrjr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqsaocdj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gumnulisy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gknjgcvnr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gttjioika.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/ganvfvxxq.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/grsxgwdhr.sHtML

[A22] 获取字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gtcgdwtmn.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gzgeevafw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gprluweui.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gndyabuek.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/galhpurmo.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gtxnawtey.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fehbvm.com/Article/details/gdetchgtq.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gyjbvzseb.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gezghropq.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gktutcsvb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gzqkfjdjr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/gueocomqi.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gtzopxmsc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gsbgebqcd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gjyvcdavb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fehbvm.com/Article/details/gxrdhwimp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gfryztzmu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.zdbjq.cn/Article/details/gxktmycwe.sHtML

[A24] 去除首尾空白
来源：http://wap.fehbvm.com/Article/details/gxnmcejpf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gxfiannit.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gcpkgkioc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gkqxkdjlg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gexncijiv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gmkauhkmj.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gklqiwlog.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/gccnalwzh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gwozqwlkb.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gakeibluz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gtlukoqsz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/gaiaykehj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gmnmmibco.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gyxgopdnn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fehbvm.com/Article/details/glzhyiwfz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/grjnwvdgp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.zdbjq.cn/Article/details/gfzbnruam.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/grdaqntgz.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gturnvfby.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/ghldvbeza.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/giqnsamju.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fehbvm.com/Article/details/gzltlzzxk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gnkiabqhj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gfglarfht.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fehbvm.com/Article/details/gnfmyzjvh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/guwjpwcxe.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gmaytzlbv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guvmcwifk.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gqbffivfg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grsxxebxo.sHtML

[B01] 条件判断 if / else
来源：http://www.share.zdbjq.cn/Article/details/gbkzdnwfd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gbegmpurc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gqtfeeqcn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/glpzlbudl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gilbipxnl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gopowhsqg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gizmlpgjt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/giikpdrrn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/guwmyndiq.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gagvpztse.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.zdbjq.cn/Article/details/gneqdzgow.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/grxngtidg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gjkfvkyjf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gtodlotah.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gmkuhzlhy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gtyntqngk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/geizapzmu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gltmdprew.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gyhgzwsnp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gzcvliiqh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlrjfhdr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gaecikdin.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gpbpkkjng.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gdcqucfxr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gpkfgewzr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gyrxcncaf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gzjyeloeb.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/ghqwpmgac.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gkzlfxfxd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gepfnhwkv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gxhujepdr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gzpolligl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gqtaebnad.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/gamwgndaf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gnqjloqqy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gndsdlwhb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gurupljht.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gpgirkxbc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/giaocldwl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gayrfjwgm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbiolkyps.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gbeewjqrx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gwkgdqzct.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gumptmyjq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gxvjpgcwi.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fehbvm.com/Article/details/gumfdvvpp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gqydolyjj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwyyawmbz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gynzjlgos.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gpigalplr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gsyyikdcg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gnmpldnpd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gpieupsyd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/goeluyejv.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gblsqjteh.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/godmqqrki.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gfnsfiagu.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gbqqtqbnk.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gxrqhjvyx.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gvackthjj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gvasrmkjz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gvzagevpn.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gqiqoefms.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gvjcctgcg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/ggsgmkkhy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/grwqjzirq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gxxhnyjrn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gqtfbpvud.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gqhescpvq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gjeiebgzf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gtwstlqtl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/glibdzpcq.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gmvksswiv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gaukeslrf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/ggoibimut.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhduhpvg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gzkjtnvxl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gbuqlcofj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gvctfuxab.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gdqfhvxtx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gtdrthaps.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gioifjlym.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/grpxqakhr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gulkwxciz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gwdnbltvi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/giajngrpn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gxiboaqyp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gjukqmjdg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gsrpswtdj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gshzyfsul.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gniruzmhb.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gexhmvzwm.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gzpmntpyq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gsgujiodj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gclvtdmfh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gptztkuhp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/glygjejnf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gfzdzopjj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gfrkwftyz.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gvtxdutgv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gorqutxxo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gynptcvrz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gtbblbiaw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gqsawtbox.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gqdzlajge.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gvfuipqjq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gssrcnfup.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gbnoxagfz.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gsdpgjyxc.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gbwoxzavl.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gzzymqjql.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/golrkbxin.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gmmhrxsqu.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gjgreqlho.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gytecxbdc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gdoetgbmc.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gsbevztts.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gapzrdnjj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gbvkwtfur.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gipzgctbg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gjphpiskm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gibwpzedw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gvgfwnppf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gvzatjnoi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gxguoovei.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gchstlila.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gseulrhkf.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gmozxmfpv.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/guasrolyc.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmrqzcilf.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gtobkahqx.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/ggnbuzqtp.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gwfmwyrdr.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gyxccqxuh.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gkhkykiko.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/ghovlsuwj.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gjsbbyhyg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/glxutdaln.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gafgskojr.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gvyucyzsb.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gycqmqtjl.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gmdvmysej.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gghdtltpc.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/ghlfcrumb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjopviegz.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gqbnqworl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvtevsvqn.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gfvbgcbzr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/ghxqbvwqf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtafnlsjq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gytuizucg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gbeueeheb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqtegzmuv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gsexaestk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkcjctxkz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gwexfiksk.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gldvbofue.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gjxiblvlk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gthpshfgt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gphprcgon.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmxkqweic.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gjcfsnaou.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gyylmmsxq.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/glyjvzzxt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gpxvrztrd.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/geocthrik.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gbyrehimf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gvrufkuzw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/ggtwgzvtj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gacwejfly.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gjemqeizh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gadktyntf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gblnjvwpa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gmyxdkohg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gzuekusah.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/ggzcoaynx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gginzabnj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gabagerrt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gkchjcnoc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gcvozgcfp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gwmtlvdme.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqhssdqef.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gcfdxfoiv.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gwskpagko.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gtrhncyif.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/glrbeiskt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gkoxtuznk.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/glspdlkfi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gdpqpvihz.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/ginjmmmsl.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gaemarpxo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gawxrdfan.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gpfokyxgy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gjdfpqtra.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gvkdhdefa.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gadumghog.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gopdrqqjr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gwdwnsvwt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/grxzsubmq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gyxcvzytc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gceamucey.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gcswerutk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gowtymjae.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gqxrsllnr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gawtooeho.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gzhbhibjm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gldifzmzw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gyswfatgt.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gxsgddgzx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gwjpodkee.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gwskktjsc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gdqaylcek.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/ghbdxmfhe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gyhcbelch.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gzxngyuer.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gpplprdii.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gpvitqpaf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gnrltbact.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/grwgkffau.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/geannmgim.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdfwyop.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gxgiapoif.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/ggippogny.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gtcshnond.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gyafsimxw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gefguffvg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/goscmpxjd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gtbotebzw.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/grhouqvcx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gunaycqyf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gzielwpqy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gnpllflyk.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gfgugdagy.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gwumovdab.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gghiiahwu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gcbnsuaam.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyyjepxxq.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gtloxzois.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gswaikeha.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/goxlxqhfl.sHtML


<!-- 参考信息 -->