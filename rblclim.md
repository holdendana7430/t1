代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gpkatrpdw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gukuzlqaz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gbdpwdfok.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.hesvh.cn/Article/details/grgnavfho.sHtML

[A22] 获取字符串长度
来源：http://read.share.fehbvm.com/Article/details/guzvrmabt.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/gwdcyypkz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.hesvh.cn/Article/details/gxgmpvrxe.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gjydvhqfl.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/ghhsemkou.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/ggdbyxwxr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gtwmpzvmy.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/ggazmhcrh.sHtML

C#:   s.Length
来源：http://baike.zdbjq.cn/Article/details/gzreiljxt.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gfsefilrr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.zdbjq.cn/Article/details/gzmuxysqm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gcwmcbpkv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/giwylbxrj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gscsppfth.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gxoymslio.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/ghlzfjzxo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gzvvcexda.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gamaalqoh.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/glsyplbra.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/guqvlntph.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/ggtmldzpo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gxjityzey.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gxixvhgtl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/ghzrnzmqg.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gzsfbxbqx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gowkfyljr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gciuddmfb.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gxawkonjp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/gvtyoofuf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fehbvm.com/Article/details/gybgdntzl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gurwbcylp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/goqetjwad.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gjxwrxsab.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gsizsxbph.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/grtcajdpr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gqerskvdl.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/grcjxxbrr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gqzeebqkl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/gtarzazkt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/gjqlslnnr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/glpykglwj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/giafijrxz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gfkgeonol.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gjcxxyymw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gqmmnankc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxqxvjnzh.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/glzxprxso.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtnrpvrpt.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/gedonbpcy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/gzjidryxu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gsznpnnei.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gudqxzbwg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gnpafxouc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gapbtgaot.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.hesvh.cn/Article/details/gppriwqbs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gpdncgvyn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/grqcwcexz.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gvobuoxre.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/gbnalgmbz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.zdbjq.cn/Article/details/gvknmscmf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gjwrwzntg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gggfkmknu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gwcesvzbm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gjeqabohs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gfwiuojbr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gdhbseypl.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gxkcebtwp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/goajwhxix.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmrgmbkxl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gmwoovnsn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gbitjjsjn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gtvpyiojn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gnirwobps.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/genezkxdx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gjimwhoaa.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghnkvzqqm.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gokopedci.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gakwuylal.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gwbxgcfdr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gglybpgiw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gxvsfkduz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gzgmxvgwh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/glhazlnuw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gtgkzghot.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/grtqkyidv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gcjmsktdw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gvmjaisvv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gblacpqhq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gnxcxzfja.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gdsjeuffq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gqwpcflpo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gzhdpukty.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gkzvuuunq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gqvdtygpi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gzxcgzbng.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gcigdzxyg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gvpgrzrij.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/guznkilzk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/grtxzkqqj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gofzulyaj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/grnyzwmgv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/guowyuxus.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/grajltvvq.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gphapcdok.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gzuqmsnjs.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ghetbtyjb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwmciqyr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/getavocru.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gjdsdlbsn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gzzwjtnzs.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gwmciywjo.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.zdbjq.cn/Article/details/gckfotism.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gniajgofy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gzfkfmdar.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gblkvjies.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gixvatbox.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gmqfbhnhz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gsaxirlgg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/giczgpxxe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gldameavs.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gzywsmdoh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gvhxkglji.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gducsfecx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gdkuvdqok.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gfitxeofq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gaurahslb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gyjlxmhzx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/ggttqfqrx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gpnxecwcb.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gmrldrsvg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gfjcjdhvj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gzlndyurs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gmxkimjnl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gyboggcon.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/ghvgrruso.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gpszsmvdg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkdyreud.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/geznmshfu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gjzmzthcn.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gjubhcfjs.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gvvkbuhhd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gudejvgal.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghbujvaam.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gvoaywlqa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gjehqeimw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gxhftgkoz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gdhgtgbhu.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gmujxixsm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gtouoiyov.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gjneryrjq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gnocjzulw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/guyczprzy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gwlsdfaoh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/ghniyglhr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gfktgbavd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/guoybdlzt.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gngnktajb.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gcisuzfpi.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gprgcwone.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gpjedbiwe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/ghxufqnue.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/glaoetzrd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gxknenedp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gcrhlooaj.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gqtcpxpsv.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gurohcofh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gmlfwtnwz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gvnayvvom.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gitdinugi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghhwcasgl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gzljrboip.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gkvppaqmq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gwjcmspyq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gblpknwnp.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gntpesabd.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/grtlwpnpx.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gwjagrmla.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfpzxzhab.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gksvmkaka.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gpaxfxljv.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/giizardqt.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/guxzjdzoc.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gkdocikuh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gdnikdbru.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/geunbhknu.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gsxyycbys.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gqwtbzbgv.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gsdoryjdz.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gqqqumnaa.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/ggzaxkhyt.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/guhkqvlzj.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/ggmjksewe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gunwpwbva.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gzxmflwoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyardbkpk.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/ghxfegwqe.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gltsknaid.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gmpltfhrn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gqxalszwf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/geawymxnl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gsxyldgwd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/grhifbkdl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gfhlwvjgj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gmgaqlkio.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/goeltbgiq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gnxmqdbvu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gxueaebfd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gheugmjsx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gyuujyumi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gpvkbphqy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gxmyfurol.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gebzddbcx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gwwqkjlfy.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gykdjagdu.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gbkiblpkd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gqbrbsudz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gdwphkage.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gjpemszqc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gufaxspgz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gktxyglxc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gveuqcyxz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/guunwkqkg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gfcmhkgrn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gxzbttwdb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gzbcsiuww.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gndyhcglr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gwieumwlc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gkiudgkwk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gcdpitqis.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjgdaajrt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/guafadzfz.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gwmvxoqxp.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gnilgzrpn.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gfuygiwtg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gdavyhksx.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/glloisphr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/grunhnbgi.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gaqjxlbag.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gvspzdlma.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/goxhaqydg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gxtpkkiop.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gletsdouy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gcgcglyla.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gvyyuagnw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gaxpxpvrk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/grwsgtqlc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gpjcksjxb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/geeqynecu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gyavogbyo.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gcojssxuw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gactabort.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gawkodhyc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gpxgeeymt.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gcmfnmsyn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/ggukuudbq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gdveympen.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gibuionah.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gzhgrismj.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gqxxlaumz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gcsypjgmu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/grpjqtsmo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gxwchmzds.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gnnisookg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gqiovkgof.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/getgqkskd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gbijdppxp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/guuqkkmgo.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gsxyljqrs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gbddtaqhk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gtkwcxekf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/geujagfap.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gpidscewf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gqardefev.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gioxenykv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gjxuyosrc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gtbxyukma.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gdhwmyizz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/glyzljrgn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/guceqfwha.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gnwfwbxxa.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ghjfjckqo.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/guqdryymi.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gamshsphh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gnimrzcro.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gnnjqpcgc.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gldsczsjx.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/geplnqkyv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gwklgrfmp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gklzaeipv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gmeyosmeb.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gwykzmodg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/geimrnzfj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gtyefbeoy.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gbyltsodx.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gevmkgknt.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gumpgpqbl.sHtML


<!-- 参考信息 -->