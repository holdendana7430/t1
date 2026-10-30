代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fanxiaobao.xyz/Article/details/glpdvksvd.sHtML

Ruby: gets.chomp
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpkrdkux.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fanxiaobao.xyz/Article/details/gsslodxjn.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fanxiaobao.xyz/Article/details/gclxeyljy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjwshsopg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwcmkcfp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gamvxqobv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvhrziyv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtcdhwpu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzxpnoia.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gedzdleoo.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fanxiaobao.xyz/Article/details/guclrxmie.sHtML

[A22] 获取字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjfeujqen.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdgtqmdw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fanxiaobao.xyz/Article/details/gnkznmoev.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfskurpgi.sHtML

TS:   s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gigqqgqoz.sHtML

Java: s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuaykmjf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gktfqjeii.sHtML

Ruby: s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfljanrsk.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqtwofoj.sHtML

[A23] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnckxuka.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtznvbmgi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqntdsje.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gydvcnpnc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgcwlrsz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gwzjmwucu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gekfwyawc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gyodgifun.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/gkmwtlsaz.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gncszpmho.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.fanxiaobao.xyz/Article/details/gytxncgub.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwocaknym.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/guwouikxd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjolsxvv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwppprtk.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwfglytf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzmvsksd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gofdyezlr.sHtML

[A25] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gpbcrjbaf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbputpohm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gizfkybvv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/giixmbyek.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmohlnhq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbclkseq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gmjizctbe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxeolsfn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtatohzjl.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/glatpcghs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fanxiaobao.xyz/Article/details/glfodaguy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjkilrpq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fanxiaobao.xyz/Article/details/gfuojkmvr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fanxiaobao.xyz/Article/details/gdazexwex.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gckjrdqou.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcybeapnk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtzskrlz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxksbunpw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzmvemxlt.sHtML

B. 流程控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gigdjrzhd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiaxwptl.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fanxiaobao.xyz/Article/details/gexvjuzrj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhfxyuyp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gicgjnway.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/glholkemb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gmsesliiu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqchztfj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbrdyaza.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/glcmnbpvu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gsrvkwpbr.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fanxiaobao.xyz/Article/details/gcxqhaveq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/gangpktfr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmuutjkc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gvtjolfdn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gtlnwhlfp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnswtcwl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fanxiaobao.xyz/Article/details/gowuxzddh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gkuzkefua.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/glzpenygf.sHtML

[B03] switch / match / case
来源：http://3g.fanxiaobao.xyz/Article/details/glcsjyzkd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fanxiaobao.xyz/Article/details/gydgivhkj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddrleccq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnmwizuf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxreipous.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtntkdszu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcyuimjx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxvlxewi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gblvaaorf.sHtML

[B04] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwzmyaho.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ghmezircw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnqrajdj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtgrvksdc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/glzohrgqs.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzavamypf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcivtxrsy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fanxiaobao.xyz/Article/details/gaanmkjcn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giktduymk.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gbkbhrcep.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fanxiaobao.xyz/Article/details/glcuefffo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqcbmnk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxkigqdj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gywssilqn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoouasfr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbswaptt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufajfjez.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshoyproy.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzyygeca.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fanxiaobao.xyz/Article/details/gcysophqg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gplcyvjsu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkbcdsf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gveoyaqsq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjxxdopx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fanxiaobao.xyz/Article/details/gysqsezxu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gennguaia.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fanxiaobao.xyz/Article/details/gelhzofln.sHtML

[B07] while 循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzovipdd.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkblwkhx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijsfbbg.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksdlaefe.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnungngzz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcgfagib.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqhzgonx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwwmlvk.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtswyosfn.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fanxiaobao.xyz/Article/details/gztzmzvvs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczuaewri.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/glxlkkcpl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gplqerxyz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrqgtfsj.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjfdjfxi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtqemhli.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmnbsglr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwqmjnjb.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/gaappynmo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqwvvnqa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmbgavci.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfwwwdyx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqsjawhv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvrkckpd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwrxdnppx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fanxiaobao.xyz/Article/details/glzamlqkf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giztodyyo.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/grupmqyxm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvdlapaa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gseyrrwck.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/grwdmvnfr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gxfwbpzpj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmbxltfs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhiodrdk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gpfzixubz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gldipgsbh.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fanxiaobao.xyz/Article/details/grqepemna.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gribwfzmc.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ggxsrgpyq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvjjgalh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzvgoikq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gkvzqujqt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/gkblwztpo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleidehtp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhwrmnye.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gkhmldgno.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gyzlpkjdc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/giicoshlg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gxivhaqpb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcihtdpbr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmidxjula.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnesursk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdgynygg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geohmuifw.sHtML

[B13] 判断是否为数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiqvpvuv.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/gdgfnerua.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqnzxehl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbnqlzay.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbcgoykoz.sHtML

Java: x instanceof Number
来源：http://3g.fanxiaobao.xyz/Article/details/glmsvcnmt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdscctvin.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkjhwehm.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdicijqa.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gstabtuim.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvophbc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/ggtttduas.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grztpsywh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbwhoojm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsanryahe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghigylhlf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvnqdiphb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqspzfspi.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gbxtfwqiu.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gkhlpymir.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fanxiaobao.xyz/Article/details/giezklilr.sHtML

JS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqywfexe.sHtML

TS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbaduxun.sHtML

Java: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmnunxlk.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gedkrgqvp.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/groyzwdsr.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxizpgum.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gttsdnsoz.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhugetsb.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guidyygqy.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtpfyebm.sHtML

TS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbbozuvo.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/ghtmdbojj.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghazspdas.sHtML

Ruby: return if data.nil?
来源：http://read.share.fanxiaobao.xyz/Article/details/gudxpkbjw.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gresxbhsu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcdsplrg.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gdftuntrs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpssdbldf.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczfkyzgw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgubwryb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghpnotjxp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gphhxbhvb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeknqcox.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqsrnuwl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvsajvqq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjposdck.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjavpomxh.sHtML

[C02] 默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlfezikp.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/glwcaqyvy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gesrbfnqz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrdccsnh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjjdzaej.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/guioispyb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gylmvinsc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfshloro.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/gklcdomjo.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmggpbrg.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/gjowlroot.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtnnzgzor.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gktqnqdup.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjehybxul.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqptmexkh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gcfetekpm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fanxiaobao.xyz/Article/details/gxhqzwbzm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gaytgvgwa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlssqfal.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gcwvgonhj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghoaycjmi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyxymxgbl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzqggtau.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfuqbzau.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gakveurof.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gspoasavg.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhagfhzu.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/glxorbjvb.sHtML

Py:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/grsqvnehg.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlckkekd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gyisnzlyr.sHtML

TS:   return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gptofsdyb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fanxiaobao.xyz/Article/details/gkagzbwhu.sHtML

Go:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gkvxfkrgd.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvmhexdx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/gyvcksymo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxayzzbq.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gxcytevqs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gngrfifzk.sHtML

JS:   const square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjdvsgkf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gdifouylx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gxptcpcry.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gmijnabry.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gkxcujvwk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gmgexnhtr.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gqdgwjzed.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fanxiaobao.xyz/Article/details/gmpoyrqfc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwtsmokdf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyguktkfu.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/gfqlwbhbj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeqfbzxa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeoysbqo.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fanxiaobao.xyz/Article/details/gucxocehn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyoyhgdz.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gklspgiom.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gcgwqcotu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwgbgtasa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/glpgzgbeq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkipfobbd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fanxiaobao.xyz/Article/details/gcmizmmwe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpoztupx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fanxiaobao.xyz/Article/details/gtqhsanhp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlmaspwt.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlttzmiz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpiymedv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukldgrqq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gwxanttnb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrykbufu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/geyufqzxy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmkgxahsq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggstrywbb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gbmxjxslh.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/grchlxjfb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbfkcoou.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/goappsycx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdscrgzi.sHtML

TS:   同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gdghnsbiu.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbxspfye.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcryuhmy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fanxiaobao.xyz/Article/details/ganjpdele.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gnasfzqzl.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/grihdukfo.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/gccacqaja.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gwibwxstq.sHtML


<!-- 参考信息 -->