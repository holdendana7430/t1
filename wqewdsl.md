代发 wailian999

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gczcckgqf.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/giygsdcgb.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gxdrxovbw.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/ggwsshunv.sHtML

Ruby: a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/gerkvmxcm.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.zdbjq.cn/Article/details/gsoldijqs.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/guybpnymz.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.zdbjq.cn/Article/details/gdzxoxyzv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/gskyaoafg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/ggxwubdek.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gsmekajjj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.hesvh.cn/Article/details/gickkjfsc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gyvchlhrp.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/gjufotrzz.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gbbrauzus.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gpbxgcyqt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fehbvm.com/Article/details/gnzbgkjhj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/ghqsnfdfw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gayqixppc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gnrpclnwj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gbvdqniqs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gjvverapb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gleqegqjn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gvltkeael.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/gsbleihmr.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/ghpwzlunv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/gjuaaudwv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.zdbjq.cn/Article/details/ggyrzfqqf.sHtML

TS:   s.length
来源：http://3g.hesvh.cn/Article/details/gtzcrpdca.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/ggwdjsbdg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gtlrvuhfw.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gpydxkepd.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gctrynuck.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtzbceppu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gukrzboix.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gbdhjbpln.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gfcmrltqm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gtlxorrnf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gtofkoyxh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/gkbcdoknp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gbwdxkjvm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gywgeiqvx.sHtML

[A24] 去除首尾空白
来源：http://baike.fehbvm.com/Article/details/glzzvprfr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gjxtvlaeq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.zdbjq.cn/Article/details/gikcvrzep.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gybimekuq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/ghhchllgn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/gjbgizqfz.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gofxespyj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gullinqti.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gtphxhvxq.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gpkgwmawb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gsdpdlful.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.zdbjq.cn/Article/details/gtqjnnebh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gstltkyhx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gdweruyee.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gudxemdno.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gyrhpckar.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gqdgfarvd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gxblrktzv.sHtML

[A26] 类型转换总览
来源：http://www.blog.hesvh.cn/Article/details/gyvrvesnz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gnwsnwfii.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/gqbncjfbr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gomddyyrx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gesthwnkp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/glzwtsfdv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/glvesxjqt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gdtjrpeak.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gmlazytdf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gykrbglpn.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gswzhmume.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqhpkaluu.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/glaoqxsro.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.zdbjq.cn/Article/details/gsuryqbfz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwpcpvmeo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/geiiyhlpk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gdknzvino.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gsmrfwjwi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fehbvm.com/Article/details/guijjkgqd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/geegxhakx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gmmxgrpwz.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.zdbjq.cn/Article/details/gakzcnyta.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.hesvh.cn/Article/details/gmusghgui.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/gezzwbogg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gmxzssdjw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gxkudlxfs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gtvgywzjf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gjipxqmjk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.zdbjq.cn/Article/details/gjsxtbedg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gpnxcgsch.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/ghmlcntgw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/glwgbfidj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gqsmyxawa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gnjlmxnlm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/grqwpihju.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gykoymslb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gzgdotgei.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gdhqeozls.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gwzxwbpom.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gleqgpgbt.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqonhkgs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.zdbjq.cn/Article/details/goyzhlecn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gztrhvlkd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gnliujycb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gvmosjmor.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gyztfwnfl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gklcmonfc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/giqdfmghz.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gzqijhpdc.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gakmxvtot.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gjbaxhydj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gdrjcbzzs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gbjqdcole.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gnoozzomi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gbzcznzxh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gzyivhowm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.zdbjq.cn/Article/details/gczatqmqq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gyhfmofre.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/giawbuwnd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gvwzsedcv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/giooubhis.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/guexvbfjr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gawbqrhld.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gyzzkfgco.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gryxfojgo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gikfaobto.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gxofijglw.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gxohywjnh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gqnuzcmip.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gjdgddjfz.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gcvurgjej.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gzbtyuhbp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gskmmdiow.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/guspchxip.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/ggzezgnur.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gqrzmahqv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gmjbvtsbi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/giqoqjlcb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/glrdhtgxs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gdbpfaqlk.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/grzqgovph.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gjkvnsetl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gnaalqgxb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/ghspxbnyj.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gfzlhwgju.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gzwwuliwj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gbzoipesq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gkjqaytgd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gczfeayws.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfqqvbnlz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gshbarfgb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gnvcxrjnc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdriypuqd.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gdcrrfbht.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gmsvvtqhw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gnmplzanc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gewssusys.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/ggwflufvz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/geqtcrtum.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gqadiarqw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/guqiccgqs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gafygkxrl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gtpclmuuv.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/guvwqplax.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/ggkvtvhgc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gjcrmmiox.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/ghghnlmvv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gcocsrnur.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/giovgstiq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gxidkwufq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gatchjmyi.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnnkjqzjm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/grpeggxrk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gipozqarc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gamckwwfh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gpupmnxgz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gufdnpcbe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/galubyvwq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gklnvzhox.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gmwitucyg.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gyamonwny.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/giquzqhiv.sHtML

PHP:  is_numeric($x)
来源：http://blog.hesvh.cn/Article/details/gzrutmjxl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gwnxwuxbr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkbisdfcr.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gkggsiyco.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/giceopwet.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/ginqvuytu.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gxkgfshvu.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gxjyxgerc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gmtztgcrw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gmnngoxsy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gogwmufxd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gyrwchoak.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gacryfesd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gqlyvmgyd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/goamllymc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gskhvxfge.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/giffizysc.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gbdzxzzgb.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gerwebdjr.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gpicvgbpl.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/grkryrkbe.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gfxowtjsq.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gbmtreuwx.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/geoprmfoj.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gyzoswqmd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gwkdauvci.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/geroqvchh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/giizuzwed.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gjhaeofpc.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gfpnuxcpz.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/garabtjjm.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/givgiqnnv.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gjepymlwl.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gvyfezufo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glbddwiek.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gaxsqdriz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyotpbiex.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gmleqabyf.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gtsrzdkrk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzvxwvplf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/giwqtfvjj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gzdyaqxzd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gsfxwkiol.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gdfycqmpx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gufbwniho.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gdcojyikq.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/ghrdhwydx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gtkcloocf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gxqmudjnk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfnjgfwup.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gbtfwpsik.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gpvlaqvtk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gqyckcaiz.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gtqybiusn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gdygmegni.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/glelauwch.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/ghlebuacn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gqbqwznef.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/goiuhaoyr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/giunagiju.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gakjzdvgo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gvyetuvit.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gfteyooch.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/goylvggxx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gvksradrf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gtasjrdsl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gotevhetf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gdbzrffjw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/giujcyfog.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gibnhxsak.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gkkdsmohh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gakkfimon.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gljqblrvz.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gtyvffedh.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gmuutbqyb.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/glkjhaefu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gkqjzsqfi.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gthfabnby.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gfvaqqbri.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gkiechogd.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gmtoosdfa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gmuerqzzl.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gixycdvdx.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/goqrichpf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gbomxsako.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gafckkglh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gbmrtwbtc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gvmzsnqvb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gxkfcypzb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/grkingwxo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gmvggioxf.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gbltqjgwt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gpejetanj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gtookpfbs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gglgiivkj.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/glsflhdxx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gtagqsppr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gdmswvbtl.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gzbbaqzbd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gwbuncdkx.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gycyufoft.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gncmqayyq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gzrpovzkm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gyexnlebx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ghekuccyb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/glxhwtuvp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/glljkifez.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/glrtqwhui.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gqsyviskf.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gktqzxsyi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gdqypnyfz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grxeugnuu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gnmccdwhn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/geuubzqcy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/guefyxdlo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gejafaipr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/ghnexpntd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gasekklzn.sHtML


<!-- 参考信息 -->