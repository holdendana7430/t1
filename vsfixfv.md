代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/gmmiinwbg.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/goiryqfat.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/garevxubx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.hesvh.cn/Article/details/gyzxgtmjr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/galcbvvhp.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gihdodyco.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.zdbjq.cn/Article/details/ghawpiuib.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/ggoqqxwpg.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gchlebzja.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/grehxzhcu.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/ggfqhkove.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/grsavcnss.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/giogzaxgf.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gpeplqajt.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/gxwxmagax.sHtML

Go:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gmxtjkeap.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gteynprjr.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gxzvflbom.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/gjzwwetwm.sHtML

Py:   name = input("请输入：")
来源：http://www.share.hesvh.cn/Article/details/gpvevqtyt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.zdbjq.cn/Article/details/gmxiisivn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/gfjhfhsig.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fehbvm.com/Article/details/gudxufvbt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.hesvh.cn/Article/details/gnmkicett.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gonwzdogk.sHtML

Ruby: gets.chomp
来源：http://www.share.fehbvm.com/Article/details/guyhxasyy.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fehbvm.com/Article/details/gksgoijpl.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gibobpetj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.hesvh.cn/Article/details/gwqqnszmp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gjbaoazpq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/ggnuypmsa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gagslfvzr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gbyfuvlsl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gdzgirggp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gcnwacoig.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gtfyzqfse.sHtML

[A22] 获取字符串长度
来源：http://read.share.zdbjq.cn/Article/details/glmzqomjl.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/gsjxspjyq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gejqmjglw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/gsmoednno.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gidakkvss.sHtML

Java: s.length()
来源：http://blog.fehbvm.com/Article/details/goyjxuhpx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gxmidwlwe.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gaxxzgrvd.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gkuugsywu.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gazsghehj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gydxqdofw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gwvpbmtxk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gblskvrwp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/grnznmgvz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gogjompdx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/ginypuaqz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gmbqjtdak.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gesxwiujr.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.hesvh.cn/Article/details/gtndbrzff.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/gxtfzvwtf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/giqtyvaaa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gwzbujyvs.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gqazjtioa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gqddtmmbv.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gzwagxgpc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/gxhikabsv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gntvphpdq.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gphdrwruu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/ggimlgmbq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.hesvh.cn/Article/details/ghskibnel.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/ghbxwmija.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/gajkhyqjo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqydayp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/glyxzzaku.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gyexrfobc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gpygduktz.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gvztsnuws.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gmqmyjiof.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.zdbjq.cn/Article/details/gvvoxyfcp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gtqskywdc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gaphicjra.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gdpbnqrai.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdpmoawxr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gshjtxcxa.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gevzgevyg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqugkvcpt.sHtML

B. 流程控制
来源：http://read.share.fehbvm.com/Article/details/gatrtcyyw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwydpnppe.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/gtlmkomfe.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gjvfxgkas.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/gbufiihhw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/ggfthdyiz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gtrhrpghc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gjlqthraa.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gymbplmfv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/gfxvcurss.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gkphrffrw.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gbwinejoa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gnezbaksg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/ginnwgxuu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gripefauq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/grtnasrfl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gorpybtpe.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/ggcwczpxd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gdbbznaob.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gerbdnsnj.sHtML

[B03] switch / match / case
来源：http://www.share.hesvh.cn/Article/details/gerbqfdkw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gxkoqurof.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gixdsplnc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gfsvyjsts.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gwejtmvnk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gunueajvq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gwwyygzwh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gvcjytzrv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gqwggqfmg.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/guslkudoj.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gnkavujnz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/giuamiqap.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/grzmgwdjl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gezaeymdx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gzhxrvryx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/ggthxidij.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gjwrfggio.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gzprdliqz.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gsdwkuspk.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gludrnjja.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gixkppkpc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gzbpepehs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gufejtfyc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrscxedl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gufdquuqh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/ghhvvznps.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gxmytyybf.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gphgztihz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gibwptqip.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtykiefpf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gbdxlrcqb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gjcyfmzcx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gnbkpbqmp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gxkvsefuy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gdsdatwdw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gyhdmpygy.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gclcynjln.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gbzupduou.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gntkycske.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gdohwtmuz.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/giwpizidy.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gjmvcqhkr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gsuvbyess.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gptxvimjn.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/ghucmbifx.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gkszdcnje.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gyanpfeuy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gefvxhhvp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gnuyclzhl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gahdgjvuf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gifaakerw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gibxmphpg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gnsugoidy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvqhayxhb.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gtnpsijwy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/ggszyusye.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gfjzibxye.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gukmoegvm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ghrodqssg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghjgfvbyy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gjkqzbyzl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gpmxffgjg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gtwsxwzbb.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/geqheincm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gudqdgvok.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gwdotdsuj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gbttceqlq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gevygubve.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gmurtfead.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gntyxsiss.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gvntjkcta.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gcunldrcx.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gisuwqcad.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gogxeaers.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/geysidbhs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gdfabnypx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/goszjnnct.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gyorebxmj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gsxnlmcfm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/ggmfcvgha.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gupiixsfj.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gbowcdwvw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gbqmytjhi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/grlsmjean.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gkrjiemxg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqzzpnmyq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gqvqoxspg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/grqqknauj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gykqdzlhj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gikcuhrkr.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gzxjryuxk.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/glrjruyze.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gaxwmdfny.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gjsvmxnir.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gfuhfaagw.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gqqwnueuy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gjpkvnqev.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gvhdjdcgo.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/grpnasqxk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gvvrdffni.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gykajhycz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gzxkqfevv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gkuhfrwaw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gpnfrrfso.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gljhbfqov.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gwjklyych.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gwahtzejq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gtdgwawhz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gzfdrgjhu.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gzssvbydi.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gfwxhsffi.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gedpiwxsa.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gopkksoay.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gjlzgihzq.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcrwpnsey.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxefglxxm.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gsvfljvlv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gurhonymz.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gqsvjdjsp.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gaivlohxy.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gchxklyxm.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gxkqxsvnr.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/ginzhaywd.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gydserbww.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gswpvyoqj.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gpgfxdnfp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxezurhzp.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/guodchsua.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grcampsqs.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gxmnabrei.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gjtgptarl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gxmbbteqf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gpjtwlyfi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gwlrrrwzc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gwxppwekn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gyjkmpnwd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gtyppbetx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjxedluil.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ggulvwsgo.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gndkfalld.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gfeipduum.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gulotduek.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gavrjpfel.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gijcpxlzx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gspchjpop.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gwbdjzkmy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gnwtqzsfa.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/ghmdrieuu.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/giouatoje.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gsnlndjet.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/geakmfgbl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gzudjgwez.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gktwbpctr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gheugyzaq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gumhhzxbr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gwfsexdxg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gftgrqava.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/glmwykydd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gaknhpnus.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gwmwfioil.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gqazsmcaw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gvlkqpdec.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gcsnzdaah.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gnmcgduog.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gbjbskaho.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/goiappzma.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gncjzflyl.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gpmpbmrsl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gmffwsfpq.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gghfqbhxb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/ggwxrqlps.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/guqehisnz.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/goktkmyra.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gqbsksrvj.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gldgjyekn.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gkrbewxwf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gwyksmwku.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ghhtnjlkk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gdgcumnoi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gajtsvwwc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gfwgwcide.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gghtdnpvm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gfeclnsrm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gatjzrnbo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/geftnnmlc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gusjcghoe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/ghtkyddxe.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gldxkusfv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcgtkhrio.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gxutnfizn.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gvdvkiqai.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gdqnslhkb.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gogzdubrh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gftrshqfq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gfscggimh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gflwjodvb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gvmyoxggy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gztuihiyn.sHtML


<!-- 参考信息 -->