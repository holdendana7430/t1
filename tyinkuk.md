代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gjwvubfod.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gdclvtmmy.sHtML

C#:   Console.ReadLine();
来源：http://mobile.zdbjq.cn/Article/details/gshbbjret.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/ggiohwlqh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/godnhrxho.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gpafarstb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gttjmwheb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gqpmukkhn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gnzgphglx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/guisjzqdg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/ghkebkdcs.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/goimdwxhp.sHtML

[A22] 获取字符串长度
来源：http://m.share.hesvh.cn/Article/details/gjjasrnaf.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gtahpzlfk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/gxkqqefja.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/guajxkfvp.sHtML

TS:   s.length
来源：http://www.blog.hesvh.cn/Article/details/goruxjovf.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gjsdxaiuw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/gzqdydvom.sHtML

Ruby: s.length
来源：http://baike.fehbvm.com/Article/details/gxbgrbckp.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/glcytaobo.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gzketuxzs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.hesvh.cn/Article/details/gduilrtpy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.zdbjq.cn/Article/details/gzhcmynrq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/groysabdq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/glgosqgez.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gpdpgtldu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gzdnfpqzm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/gbkufzyzf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gonwnyfty.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fehbvm.com/Article/details/gnktqyruo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/gauhzihga.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gzicqxeey.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gkyztdbss.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gmbtrsblf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/gsxthzqid.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/guuyzhegq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.zdbjq.cn/Article/details/gmytnsatz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gjqwgmdli.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/ghdifbzhq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gmkqrbuwn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gtghdtped.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/glhhhzmnn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/ghokwnsjh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gturuxlzy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gdpvjbhcp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gstikhqup.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gwxjcdhjh.sHtML

[A26] 类型转换总览
来源：http://blog.zdbjq.cn/Article/details/gxkqjfatv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gndlmqnol.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gzodvuqmk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gzqxfbtkq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gdzvewjbq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gseozmxas.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gxhpynurw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gzkiwuxbj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gjwvagrwx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ganuzuken.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gmkmgexvc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwtzhnkea.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/gkooornko.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/ghnibxjtp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/gbglnxgyu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gmxkdrpey.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gvienupwc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gcdmznwlc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gmsvpnjpa.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/garmwihab.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gchqrbjco.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gtuuwcdly.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gqnlbhqnx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gclwebjad.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gmyckbcvy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gnrxxfdfz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gxudxbbql.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gwhvjspmv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gsxbbsrdn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gytnfflzn.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gaheflhta.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/ggahxhede.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gjvlytcfw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gbppdimul.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gavqhfets.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/grpilhzwo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/gsvurjyih.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gugnmbzpk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/grausgtfm.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gnikdmber.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gxfustwps.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gktzxucmp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gkyfqwmkr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/glrxfjehe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gsxbtsaly.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gyjkcaufi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gsxiolzec.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/gpynskcpv.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gyprxfhgr.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gginrdtoh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gdrrjdwkl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gkjybncxt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gffzodand.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gnrbrxvhj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gopvcakeu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/givdsisif.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gqqnsqeji.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gykcavwtx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gkiokpsnx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gjvyiqndv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gyzfkawet.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gszcwghoq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/glhcynfko.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/golbnyglc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gpntinruh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/ghoccikuf.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gefhgtqkd.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/gaqryruse.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/grqdrzlsw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gnzkwjawz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gmpwmazgr.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gmcoyhfwb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gyorhyswe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/gjlzthbtr.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gpxnagacw.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gzhtwfouq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/grsokspdk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/getcrfzmk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gfyxgkxvu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gjfcicgpa.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gkojncddg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gefifyjtx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gznymvalz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gjvxczffm.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gshqirbjg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/glrjrmrjv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gjaonlkpq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gvhchziwn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gduclcxkt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ggdpkuwab.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/ggrxhnjze.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gmvzjbllu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlqeckyv.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gmzhgosoi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gfpigdtti.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gaxsokdid.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gpajmwqeb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gqecyxtem.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gskxqxipi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gxvlmrxcd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/guxzoibhn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gxjietcwt.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/grmjwkymd.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gwqqilbcu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghsjeyssn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gybdyssew.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/guasedhij.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gxykvvuqs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gwamzebwy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gzztewmsx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/grojyopha.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gssejbajq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gltpubueu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzoyykdaf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gwpzyocpj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gkyesbnnp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/grtvqtahv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gvglelmao.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gcpztbyqf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gydusrqyc.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gxgcybzif.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gfkibswva.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gsogbonpu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grlzejaxw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gunyxokiq.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gxftqfmps.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gufnuagrn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/guztehrnv.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gxpaisklo.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gnczzijju.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gwhlroafr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gnxelkquo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gevhflxmh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gtuojobnv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gffbpyweo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gowsqjdgh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gxogdcmvj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gdoytiqkf.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gugsjtpli.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gbhyfzqml.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/glxjyogmr.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gqvoorqmx.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gsnywkwek.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxijnarwq.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjuyqsutg.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/guqxvpwmx.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqiuzhzab.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gkfpbihev.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/guczmbfgj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gdcecmtfv.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gzkgvyjid.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/geksbjazm.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gmflrfola.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gfafubhxp.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gtboyxjhv.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/geqegifnv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsqhuyxuo.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqqgdpqkn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwvalierh.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gyraszgtb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gjrxswwfn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdkmgcvpl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/goeksbpuu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gaqurbawh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gudtsswdg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gnrstrhup.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gcgfjtkle.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnlwbrwtf.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gbxlxyidm.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gxrtbwxbv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/glfslnknz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/grwyuibfr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukoybhmy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/ghxilqwsg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gejkstnuk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gpehemjnf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gkzliixei.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/ggfwfzubs.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gdlktvtdj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gimxqibpt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gscqocsie.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gudmbffzc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gycmnuyzh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gzxetfxal.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gqxhbmegx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gsqwqhebw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/glkozwviq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gronmqqso.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/glvboupvb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gicekesvc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gzackaxqw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gmehvwqnz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gtrlhfmog.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gmqfkbxko.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gomzosjsl.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gycqonpka.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gmyhwqxks.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gycdgnyfz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gqqtfbqwf.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gyqcwotco.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/girdiuxvq.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gpcmtxdch.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gnnaprtbo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/ghpwzirue.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gvzjltibm.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gfdttbqek.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gtettmgzf.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gthfbpmtd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gzvsbxlbv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gcvrxjyrs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gdzmmnzdt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/grkxpkzkr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gksqmtklr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gvhyslskn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gpvgoyxjv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gvnqkbfib.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gbvwjiwdp.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gbwoilnfv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gaednpgxf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gjeqdzapa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/glqfbpbvk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gkxtwutpo.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gkzskebne.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/guybdugoq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gmqkndhsn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grfnlgsjf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gdfuccfjf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gvboyddia.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gwuevenfu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gavpxrucr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gyhpaskor.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gkhwieqpt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gzzqiohia.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gpbodjpsr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gykmaiwyk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gylyathtr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/ggjfeuwyk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfezwkbwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gjvdulcbf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gxjpcbsai.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gjqrkpcjn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gnahlymwp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gyqyvvkan.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gnefyqiuu.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gxklbfbqh.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gjumyijja.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gwqecysux.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gelsspzvp.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gyyvfqipj.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/grdlpmjlg.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gndugusal.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gukwraacv.sHtML


<!-- 参考信息 -->