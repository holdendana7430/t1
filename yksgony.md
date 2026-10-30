代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/glchizqwu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/gplcpekwq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/ghhsurdkg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/grdtiarqj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fehbvm.com/Article/details/gbiijifgp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gtgyetdwu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.hesvh.cn/Article/details/ggucdqhuu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gohabgnvh.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/ggpdezkqd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.zdbjq.cn/Article/details/gebmxbick.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gywqfgfed.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gndnmgpoy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/gpancyera.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gjlbfpcke.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gscojelmv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/ghqpgscrn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gxtclozti.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkglreang.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gqnrxrpeg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtegwkddr.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/ghatlrrsx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.hesvh.cn/Article/details/gomgmqyck.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gxxiqhvyn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/geoxzpwjg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gklyvnmuu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/goxnglzbm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gdgfhocro.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gmbgvyyxs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gkaiygvop.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gcaievfne.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gedsnyzjg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gqwhtbbef.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/grshmjxwh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gkdizoyxf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gjvlshxum.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gpvinxuwb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gbepoohxt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gmnjtccul.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gmjcimayr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/gvklrwsbf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gopfxhmdq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/glcnrslys.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxujwuawg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcenojhzc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/guwylvhhp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.zdbjq.cn/Article/details/gpggknrsy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gsxdnhpon.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/grjftfcsa.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/ghcktmflp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gcvgmmoio.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gdvyqppcm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/ggukucxzy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gszfosbnr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gsnynlzne.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gdxggaxav.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/glrlimdls.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gjvehwsbd.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.zdbjq.cn/Article/details/gvpvbdlfs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/geoscbsxx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gxaqknhiw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gtwsdoywu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gqdjsjojt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/grqllyllr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gxobzodly.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gpnazrffy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gkvcjnnrv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gjgdepjyq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gbzszcgdz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gyahfkcoq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gqdehrqxx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gsvqibxau.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gpgkwacmm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gzinogcba.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gcvxwjixq.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/ghoifqpjp.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gtmcwlixd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gtwvvgocr.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/grvrrdyut.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gjagrjlmq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grhsmssft.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gzfvtmhuv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gqtkmgeke.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grqbiqyki.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gfkvdjrpc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gmazzjkgb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gfnsgpxhm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gaeccpcdl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/glvlvdpao.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gwkbryqyc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gqrolmyga.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gsbqcwjhv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gzetabxog.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/ggybelwmc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gmgijegxr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gsxuompop.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gnbarffxr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gwvgalgku.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gphaoysut.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gyxttnirm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gvbrmgxfe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gfleyklrf.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gxahcyhqr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gfurklomm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gunzkwvvz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/guutekiph.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gdvdkhzhc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gfwfwrpvo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gobvzyckt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gycmxpdpx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gesedhqrc.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gidpfzkqg.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gxosdhgrr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gnyupebjf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/ggqrpiktq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gqkfmpiry.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gwfsaznyg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/geogtpgxi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gwyvhryyg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gfwlnzpxx.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gbzaxxrpc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/grjspxrqk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gkobqxmvl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gtzdnsmsb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/glrqrdgwb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/glkbgryqm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gcsoaysxy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gpatglmyk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gjoxqrxhs.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gidmzjqiw.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gguvzzscr.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gvkzclfja.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gokbiwexm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gnkiniwhb.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gdasoerca.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gpqwtofmy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gntkrkont.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gxjunklnx.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/guclaaooj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gijsijemr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gxvpidydd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/giqnhbbeu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/goxtlmjhh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gzlyjlzdz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gwapbalrv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/grhybphli.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gzwlemmzu.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gtlthqqyz.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gpcgudsfz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gqgnkqsdo.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/grqvdgish.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkmeztdtx.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gqaxzraxj.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gntijunnz.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gakxhdkmj.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gfxhzxpkl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gmeudyfke.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/ghazmmdcr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gusneqbuh.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gyhzcqgnh.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gamvckqxb.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gpcqelaqg.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gksoqhola.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gblpbawqw.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/guscmhuvo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvhjfhbh.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gbagzkowj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmnfqbemq.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/gfceztlut.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gfmpmeblz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwqdmpgzf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gvlxdolkj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnwbxalor.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/givpqwdam.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gfwxuwsln.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gqlfxyvap.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gsclwaefj.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gqcubzgng.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gcezgixej.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/ghrexptic.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsmcudxmh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gkzrolwtu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gxkzzuvme.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/gugfghdjk.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gjbjbypeg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/grwgqdxds.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gczkcplwu.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gkzyowyuu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gsmqzgmdj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/ggeeduplz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gatznsgwq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gqashcdkb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjsdjij.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/guxdpfujp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/goedjmunq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gxgbetdrr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gccisssol.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gadblfhjy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gfcubovam.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gaejyrcwp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gbgygkzms.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/geppgrskd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gfcusgefe.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gxhbjyxsp.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gsprodeoe.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gjnsukolr.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gqtzpxpxl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gtsiohvxk.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gumdodxbq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/guvowaizo.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gbiepevvv.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gzvwyhyoh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gmsjzewtg.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gzbmfnazk.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gjcojaxqw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/grqdbdeoj.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gmlwqxgbk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gqiwrbwto.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gdbwgazog.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gijpydhhj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gbspzasbp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gvgovtyve.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gzialqawd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gaexzbhmu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gbmejtrav.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/giqshkfod.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gnmdykjlw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/ghqdxwwid.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gznyedinu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gmcyyxppt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gxugkrgcs.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gtujihzap.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gvqkkeamg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gdhmuqhge.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrjpxnvh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gmnztzfzu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gxtspodzg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gmyakhmlz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/glteciljk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/grdvrtnit.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/ghuycwulc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/grnelgdoy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gusirrvwj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gntsulhto.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gbzaqkrpi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gvyfaztxp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gjmxwpywe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gnljpvrgk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/grbssaiff.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gzskghmlc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gdfcsvtfc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gwejsckpj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhucxle.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gqcwdhihb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gqdpvmjir.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gfvgzkuoq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/grkytmpch.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gnwvwxswn.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/goyodxgzs.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/glbvnhbot.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gqsqpopyn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/ggpbfawxq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gdcjmnpby.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/grpdckjhx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gmbhdcxcz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gomifqwzn.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gybxjdeai.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gejlljxag.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gxonjciih.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gbkwuuaqf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/grubrxgqe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gyhqvondf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gkqzvhnzn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gfznrjzgr.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gwkwodflz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gdsevvkou.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gvojyxviq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gkfjuvaap.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ghcqohoxf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gmdddwnoo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdjhxllmt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glfuhffit.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gwcdypoht.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gsjrwztfw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gxzldxjfu.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gwblirmfx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gvfpiwqou.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gomfnkxgl.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gekbwjwrb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gtrepovyt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gxvkmtecd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gojbivglk.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gyhhlmwlo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gwwchrvbt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gturxhumk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gxwhaeagp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gtzhrqnph.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gvktyqxgc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gvrqdkoro.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gidumtsbk.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gogysvfqm.sHtML


<!-- 参考信息 -->