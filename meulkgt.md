代发 wailian999

C#:   (int)'A'; (char)65
来源：http://m.share.zdbjq.cn/Article/details/grxervyid.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/grwspuuhq.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gbnatspar.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.zdbjq.cn/Article/details/gsptqgauk.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gievuhcpk.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gygfjgudi.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/ggjfjgyfd.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gdurwjhze.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/ghdnmnigh.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/geuicrqdb.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gzdxggpqn.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gglupasmb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gnzkxsrpc.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.fehbvm.com/Article/details/ggaheofrn.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/gdzrnmkek.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/ggiakmrfi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.fehbvm.com/Article/details/gibydkltw.sHtML

Ruby: gets.chomp
来源：http://wap.fehbvm.com/Article/details/gpzzbbsfn.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gwuvzlmke.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/grgjsqasy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/gcuwgrkcr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gvnhapmyx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/goqfcikko.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gcabfeqmc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gnguxsvqf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gyayrkbhl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gtgmchjwj.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqipramx.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/gntbxwbhv.sHtML

Py:   len(s)
来源：http://3g.hesvh.cn/Article/details/gbykeeaud.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gvfiototm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gifpjvskl.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/ggxzwjrms.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gkcbdofgs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/ggfhkkslg.sHtML

Ruby: s.length
来源：http://www.share.zdbjq.cn/Article/details/gkroshmdz.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/guzrjaczp.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gerkgkukz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fehbvm.com/Article/details/ggtejcmqu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/grvyabvqu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gepmiehko.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/ggdcdzlen.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gnoedysyu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gdticmttr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gpxrirqlo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gjwwxfqxw.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/ghbfmzhtg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gcmduearg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gdiycbrhs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/graszwgmt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gtxckcocz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/ggsdujmtn.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gxvkuahjv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/grrxldahq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fehbvm.com/Article/details/gauixkmwx.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gabvzbohs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fehbvm.com/Article/details/giffmmren.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gmcvjdcae.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gksaiqpxj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gabodkbhf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.zdbjq.cn/Article/details/gwszkusgf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gpfaospcm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/gwioylxem.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gqxbdvqpf.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gcywsihkb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gusksnoov.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.zdbjq.cn/Article/details/gbixerheo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gmqyjakjf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gvibvvgih.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gxarfywnc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/gwmtbbcou.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gfxofimqh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gatzcmrby.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guhwjcksl.sHtML

B. 流程控制
来源：http://read.share.zdbjq.cn/Article/details/gobbcnxsq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmyiwsaol.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gwiohlbnl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.hesvh.cn/Article/details/georczzbs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/gqvxykfdm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/goucbdzoq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gpfmdeybz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gqojqbuej.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/gplaubwwc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/gydphbvzw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gavnzzrls.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gkkmezjyw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gknjgmdmy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gtrsctrjv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gggikwbbp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gfigywezq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gnwowuevz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/glmbdyxvt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gsejsgwur.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gwjbgalam.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gxtqfgrqb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gegdayfgz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwndhemvq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gxitxlrdb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gmgzbatkn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gdexdkrcp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/ghtxstnry.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gdmrmleit.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gmhwejebn.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gkwowrndz.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gqkgerfio.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/girmxxdrq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gxzkdgfcx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gutopwmve.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gpevctiru.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gouwgugex.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gjiurwhkx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/grcmcyhak.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gkxnsiche.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gyvwohoxj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gxcpwljaf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gcvbtybji.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gjdqayivl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gpggllcav.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gaxqchhvh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/glrbllbca.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/grtumxnky.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gzqzgfphg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gvggpwwyv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gnrzafhnh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gloipmoup.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gjttwilcw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gejpmzejm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/gkztzbhif.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gavppcvju.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gavsnzpyd.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gonuxxdni.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gynacgizh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gswmbwdni.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gqcafgujr.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/grlabisfi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gtqnqlkhh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gdiknqyfr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gdcsrhygd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gwauklmke.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/ghmfqgbuy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gaixwigek.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbnrnsuzr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gacojjmxs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gsbjdopti.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gmrrjvlos.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gwyasvgus.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gzwuvusiz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gfwzslnrg.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gjxiptnqy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gwykkzhty.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ggndwzgff.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/guhtzorvz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgtlcbzy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/geqxasnzi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gxtvwsapo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gwgiyjoat.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/grmsglatp.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gveqqzoon.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gxbhaldyg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/ggfiewfby.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gwziqswkz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gbnkrkxvd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gfifriwen.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gsednnivs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gxmuacynj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gnjadbwih.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/ggtgiwiiz.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gvmtfpcch.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gudrybbeg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gestoient.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gwcqvtltx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/ggsegndww.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gczxhdxwj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/ggvstesfx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gyoskimgy.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/grdqltlha.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gignktczl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gefsofkpw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gtlpwnxew.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmpkzdbvf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gnskyoqyn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gqxnzzcoy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gmsggofqb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/ghstibjux.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gbmyighmn.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gkzzudodb.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gsbspybju.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gbizhxqno.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gotkwhgqf.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gzzlxfdkt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gyajcwyta.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/ggirvlgrg.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/ggupmzlne.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gwfesrvlp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gevhlvkeb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gnclzkczg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gofxlzfxe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gkjmeuevj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gugekkfgk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gzrvgctum.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gqisslflm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsfixazdt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gupedymju.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gkfpcysml.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gcnszdwbf.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gwbcqhcss.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdsrvfisv.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gynegipvg.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gnrkafelq.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grlgrtfdf.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmmlfqbiw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gzkcagmoc.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gthepbaxq.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghylcpqto.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gjujlklwi.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/ghiimnoyk.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gxacovvvg.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/girpuncbl.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gcrgsxqpg.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/grfcxlood.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyisuxphe.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gtjbtadgw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goxyjoqtf.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gpvqsvexs.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/goqsyustq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxmvhzhvp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/giycuxtdy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gilfjetit.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gbnhuwwtw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gwqpejcrb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/goiqekuby.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjrhwsxdc.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gvzfbinya.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gngjpqgtc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gmakmswmb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvhnxjvet.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtwdhbdvt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gsyylczvk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gsgrxxmqa.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/giiwfrmbp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gxxxvucqf.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gohzkwsvt.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/glbpmmvke.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gftngwfbg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/ghzrptvge.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gkeqjpalu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/geqlaugjm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gaeihpzgg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gdiujlpuy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gjyahtmfx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gjcysiomg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gccybdmse.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/goqeuvoxn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gxwgklunu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gcznanyqm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gwwaxohco.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gpodvujlo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gjobxmkcj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gobvfqkxe.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gnlgjkyuw.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gtsxzfakf.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gwlodsgwi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gmxoijsiy.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gkjrrqjnk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gfsmgpidz.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gkwirqeuf.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gndanyqqb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gwnvtqktk.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gcmbuyyyf.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gtodzisxo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gwyrmgmto.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gzgfuitvb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gnbdyiodn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/ggltolhdz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gfxudkiyo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gsvuwddik.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gvmmbicbw.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gfsayhuao.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/ggddzpcrw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyzwfpkal.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gpjocrfbl.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gnwqnppfc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gswpfmkvl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gfuqkyysn.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gesrycqwi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gjulpqrmn.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gchosocns.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gfuuvqodl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gvtpfmhjd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gtzzavmkd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gievlwglf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gtmtrryhu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/getvhqjri.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gtaqpjkym.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gktjwucyo.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gxdjjpfxq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gunqjmtfu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gfhbqmbwj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gevwsfneb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gjdoijrya.sHtML


<!-- 参考信息 -->