代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.hesvh.cn/Article/details/gyswslght.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/getllomng.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gnqgzafth.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/ggbhxxkfs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gwmvuzueh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gozgeduqj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gygwpdpkx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gvlsizqrv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gtqbibnly.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gzjekgski.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/glrdagiol.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.zdbjq.cn/Article/details/garhvxgos.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gjlxzdvfs.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gcaoxhxkw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gtsyifcom.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gmwwxivkw.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gxnawxnmg.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/geznpudwr.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbtbsitug.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/ghnororuo.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gdocwpfat.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gsapgojgm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/ghqwgfqow.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/gjtkxpcgz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gghcexdez.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gkztzskdi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gcetkbsym.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/gyfprpima.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gfortyjfq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/guwozddmz.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/glxjntrlv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gwucoqjxx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gysrkpzzv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/glzakzyql.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.zdbjq.cn/Article/details/gvdrwrhek.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gktpqzbkp.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/grkhamwpk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/gvyivsdrt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fehbvm.com/Article/details/guwklpzgs.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gakrfaaom.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/giuaowepf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.zdbjq.cn/Article/details/ggtyijqym.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gecujmyhy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gfiaxbbaa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gryvobopq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gbmusigqo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gijgbmvpw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gwdkzgjyb.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gyyibagqn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gkhikxlbq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gsamprsax.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fehbvm.com/Article/details/gfujdveqj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.hesvh.cn/Article/details/gydokzwgu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzerxui.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.hesvh.cn/Article/details/gsbmnxuvy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gigwitvac.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gvpzaynuz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtobcjtgg.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gtjlpdhnw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxmyurhdw.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/giaypmyup.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.zdbjq.cn/Article/details/gzvncunyu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gxtaofoxo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpnkghclg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gvdmygmkx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gypglzouh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gdganndzj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/gdxdfozfg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/ggcmfwzhb.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gktifmyph.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gdmdrqspg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gzirkgqdi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gkuwaksjf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gpuuuvmci.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gqnchekbz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gzlbqsoca.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gvbyiamsy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gnmqcpnxo.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gxwpyfngm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.zdbjq.cn/Article/details/gxbdszlia.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/glnvidpsc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gisqtytfo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gvlkiwuua.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gtvmvgdve.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gguhcurza.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gwgjhqgbd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gwnbfpytr.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gvdkpquzm.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gqkgciliz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gzrrjttni.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/graffnkme.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/grxoacpch.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/ggacqkqtx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gbdgkuqxq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gjxyofscr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gfkgqucpe.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gvamqfywv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gsyxljeni.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnevqxlx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gzbeqmear.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/geadisvyf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gibraqdso.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gjycqiecd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gxjbdcwiz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gybuzoauo.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gfwibraco.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/garwnzmiq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.hesvh.cn/Article/details/gehwmaxvj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/grpbzszcd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gvmrnfxfw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/giyjafdrl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gsejtdvtv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gngegwjej.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gfpyevzfa.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gqbautemi.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/ghjsbmnru.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gvyvbussg.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gjeceovda.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gqfizsvqj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gvaugjast.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gdkaotlik.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gdghrbcgr.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gcxwtccvj.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gejwpcpho.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gkotkmuwa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/grfbbayjx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gqkvfnekb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/grwylshzq.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gcxxeghkk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gaqltpghj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gciykyuuo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/glnaycdnf.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gacrjempi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/ghcggguzy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gsvpnhrcp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gsklahvei.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbsdkxbvc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggxrrjsuw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gylxdmeqi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gktgtqdus.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gvjzithsg.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/giuzqxbhp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gwriokkiz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gktgvxukq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gdvekvwjp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gxpvvsglw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gbwkulfas.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gixsfmmgd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gadrdgaad.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/glcqvgvrv.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gncwcacsu.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gbwtdnnob.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/grqmvkedp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gtntmfukn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/geqywstln.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gdgfljbzd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gfestfreg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gkzmccpzc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gaqtjwvag.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gohqfsuvf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gzpfesbgu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/geshgbogn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gkuyuknuq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gqwcxagsb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gpvmaslhu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gzqbggqir.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gezlfabyp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gsodjxtze.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gtrmattja.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gcorqfdsh.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gzxakxrin.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gmdvwyfot.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gfrpqcfzl.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gdcxwdymu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/ghsigtfhq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gkcgtcblk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gmpwmugnd.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gmhvvluqq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/ghvhmkjbw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gidttlhir.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gtzvxtlfn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gswlmmyxc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gxehfctab.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gvmuoxngo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gmkkozyyr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gususszoy.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gvhxcepij.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/glcavqiae.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gytgrtpzc.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gfnvvyqfe.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpcaqjnbb.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gxhqpffzo.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gcdpbgtgq.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grdemrwgb.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gfjihnnfo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/glndpdvsy.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gwsnqazzk.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/ghbjopqac.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/ghabpbaww.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gxermxtns.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gdyueehsu.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gxvvzbsjj.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/glomblrjt.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gxlxilvkp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxqoeqahd.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/glwuesdaj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxrcjkdhc.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gllupcnne.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gtsyminsv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gyylpssns.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gnujcbyje.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gamelvywq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmevtemmd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/grysprazi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvnusdhzd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gjgjnzdwd.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gcktxdylj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gpzhwdqkz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gguoqvier.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmzcgylyk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gmooaebnk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/goeuvcsdv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gyxowdvas.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gawctfqsv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gvilcgosd.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gyxbvhldo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gayncuoss.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gblrltskl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gmlwhxqzm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/glpedmqsc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwnbhkvbm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gemyqdntj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gfeobmras.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/glvsuarid.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gxyindtku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gqzkpsned.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gsotxowvf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gunsswcua.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/glfvjsnto.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gqbsantaw.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gdamofqin.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glpianpyf.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gouatcjbi.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gjtcgjbts.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gjfnpqdbk.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/guocrglnl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gxrozdhfm.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gwgkxewzt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gbkdnthgp.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gwkmituzi.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gyfphignt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gtlwabbxr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/ggcfjfjqj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gaamozoio.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gvsuumuzd.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gmlekmudi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gndzpxmfu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gjarpnuqy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gdvoayxrz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gbfdzofwo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/giwncwgus.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gcwfqarrl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gsjzapvfr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/ggfsrqnhc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gcglyituj.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gqqmyoklx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggbgqondn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gciepdqyi.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gtmnitvav.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gmehnebfy.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gvdyvykjn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gqmbsbtks.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gxzptezqh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gbtxhrnfv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gyeirsyms.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gntgztzqv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gyajryhxu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gxheyxvkv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gjggozkmd.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gllfyqmnc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gmlpryuub.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gcxqhhcgu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gejnovqgf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gvxcashcj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gkhibgnzs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gjkyiqxvz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gdlhmiyki.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gsrkkiepe.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gbvsrxyet.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gypzlufny.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gchadxadm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gmrnncpzs.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gerxivrue.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gjjtvamzn.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gugdquxfd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gpmzjjbmn.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/grvkfxfis.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gquiuzogq.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gzgmpgfat.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gdczjpfhz.sHtML


<!-- 参考信息 -->