代发 wailian999

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gzoyzuuie.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/givbsjfro.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gyzpycuim.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gvyavsvcf.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gjntmeytd.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/guuhqbjkf.sHtML

[A20] 读取标准输入
来源：http://blog.zdbjq.cn/Article/details/gosgldjif.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/goxdogfiv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fehbvm.com/Article/details/grvhsddsi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gqqarsgkj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gpdmfsqah.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/gthnhslyl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/geqxtrssx.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gkgqcutwf.sHtML

C#:   Console.ReadLine();
来源：http://wap.fehbvm.com/Article/details/gxjmcjxin.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.zdbjq.cn/Article/details/gcybdvmov.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gcilxnoza.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gpxwvgbcc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gujswieag.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gwyazxjdd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/girxcmqip.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gcpdztaig.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gipklczpm.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gjktxslfi.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/grjadzjeo.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/gvxyecuhv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gkexvqota.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/gmllrzhee.sHtML

TS:   s.length
来源：http://wap.hesvh.cn/Article/details/gjvoaawkt.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gstizymsx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.hesvh.cn/Article/details/gynfofzdv.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/giutvfztw.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzgrsdjcx.sHtML

[A23] 大小写转换
来源：http://3g.hesvh.cn/Article/details/giubgchfi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/gnjrhsrcy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/gujssvehp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gerjvkvfu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gwtmntnmp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gbzrrrtad.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/ggrslytgu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/goddcmiqx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/ggvfpsuhe.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gcvyejqgi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/gcetnetzz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gwqsnhpkq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gcgwzzhgf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gzxkdnzhy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/gszpqnwlv.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fehbvm.com/Article/details/gimzfzcbb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gzvfvvmau.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gxbjojiju.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gcwrjeiao.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.hesvh.cn/Article/details/gdoxoacwp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.hesvh.cn/Article/details/gdsjkzvyr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gbjcegwbv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gntdlguab.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gartkbgal.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gomoxnbvr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/goppovmgd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/glatcuzmc.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gwcfqguoj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gbbmitvkq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/grwdhrmen.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gjbuczctp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gtcivjbkx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gdgjowozt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.fehbvm.com/Article/details/gpwntqygu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.zdbjq.cn/Article/details/gbhmsvikn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gunvndyoz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gphluvysm.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gnevvymyw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghyhavurw.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gqczmfuaw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gwjgyeszy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gshwgfdbr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gtmglvkvn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/grnuyiswf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/ggzclvxzo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/ghybfxqfw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gliovdyrr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gthfalohg.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/guqgmxqgb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gmrrufszg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gtslmyhcj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gylvbfmog.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gpezegqmn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gxrbqptzd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gblfkdliv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gdbuqostg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gkweuasbt.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gxgrrvxtd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gidvvypxq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpujtalwz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gdqpxdzha.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gdavvdnde.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/glnfulteh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gzbosqema.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gsgfsdjcx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/granynldu.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/grbvglnve.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gotqylitr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gqbnipqkm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gjcxigszt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/ggxzcifuv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gbkikqutf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gktnbmiee.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gboaaehsb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjzirfpb.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gkyucppjx.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gybxutskq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/ghiiimxvw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gmtablbvv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gzanwbeee.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/ganykjrdd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gzhkaeqsi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gikhjiouw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gaiwctmkd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/ghxqakoay.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gkzhsnjbi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/grzykjgqb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvuxmdow.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gpulccrhs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gchkmsjsj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdgyviy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gvnmtlzmn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gcktgvzdc.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gskjgpstr.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gdzifxfsm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gnbgreobv.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gtfuppqkp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gobssuvcn.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/glwhyylze.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gjuhihpnk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gwswixetu.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gdkrejdlz.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gifmwvqzr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gszchgfnq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gppazafzy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gxsxddnew.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gxsqsrnvd.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gmoboiskd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/glelqbagj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gadarvfip.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gjovjzglu.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gjuretdnq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gbrvnpslc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gjoxstuzd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gkmwrtcal.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gvasumcqg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gsuokxezd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gpzgdezew.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gskflmyhg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gzqnkyxss.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gjjvgmyzo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gymnkpkyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/grmqepfcr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gwwanaews.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gffcaakcf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gmurycani.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gxwqqqrna.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gnkjqkfhr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/giejycgpe.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gvaisbkcn.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gdxjuinhh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdxaxczku.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbqhzqdlx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/ghvmchuxf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gwdxwuxok.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/ggvlryamy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvlzwfy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gncrgvvew.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/grtfjgoqh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/ghicpphqo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/glrnnggxz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gtggtkfal.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqthusjqf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gyfeukucu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gziakbrhp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gfvlszuna.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gfnythiwk.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gwdfxpqyz.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gvwkpfdhc.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gdlcoxaor.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/glftnhysu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/ghlipjcvd.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gjnqcwysv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gaqtpgiyk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gvextbvur.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gtsqrjifg.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gdlkflgej.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gvwkojxvk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gxecdxsno.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gzlcqpkmc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gobaihqzl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gxkncvdco.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gnbcjcjse.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/grvdwcoky.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjgphuupv.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gortsgqmt.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gmsgsvzwx.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gagsvknef.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gqczgaehr.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gphpijdlo.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gefwpkvzh.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/galwlpxgp.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gkdtgaxth.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gviwbhehx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gykcqruon.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gjebereyo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gkwdtmnku.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gfybipeoi.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrigtwzw.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/goktamkto.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gfviicwkq.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/ggogextrz.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gatafwzdy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gardaslra.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gqdrgmpaf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvxbybykl.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gvgojlsfu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gcmktrsqb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gflmdunoi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjmymbdng.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gyvmgojal.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gbjwocdbp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gncyefkrq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/giiqhzauz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsuxwsort.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gwqzuduai.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gphshhgpk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gzwxaxplf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gaqavjjff.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ggoaebwgd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gvdvwtway.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gpwrsqplw.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gatfrxwqn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gkfxicfku.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/ghoovgrbo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gdoevrjul.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gfjkjwzba.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gdntddnvt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gwnivkcdv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gwmsyyhqv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/ghzyulivm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gfcklsnpw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gviytezom.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/ghgcsccrx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gjrrykofs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gmbynpalt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gqfwbizzl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gsigclyri.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gktbramgo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gltifheaz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gzfoftbkx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/ghnqvcvmr.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/grockhlyo.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/ggxjzsurn.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gejaeyztx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gkuyddorn.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gwtnzwzha.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gbxanomfq.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gelaadgbv.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gxrucqezy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/ghlyymtfq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gptzgveyj.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gddjpylsy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gnbvrynlh.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/ggrfqxljw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gekrrrwrs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gglwlxizz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gnuhkwdeq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gdhxuylis.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gcrnyowbv.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gssrmkknu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gegqeitaj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gdsdpxfgg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gbynhkake.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gipucolgn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/ghjrgtzrj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gmfsseppd.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gecoxqyju.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gwuwzdurk.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gdaqpalsf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gpxghywvt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/griclenkx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gnghbpkjq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gagcnjjcm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/ghexlztvn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gbzhjvyrb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gjfzmnawe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gsskvhuxk.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/ghcypsfxd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gabmigivs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gvbffwakc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gqpcuzezj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gleuoamss.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gfjtziqfj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gurcusmrz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gkthiqtbr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gkqhcmyuk.sHtML


<!-- 参考信息 -->