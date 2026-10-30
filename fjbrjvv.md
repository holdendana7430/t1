代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.hesvh.cn/Article/details/ggtrnsahu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gdizqeuod.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gsxvposho.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gdyewuojz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/gnkowxjra.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gvotgdeep.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/gvwqjaxmg.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gilpzevvd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.zdbjq.cn/Article/details/gwfztecle.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gittoeyxn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gwuvtivie.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gesbkuckc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gpifzbivq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gywichide.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gfykzrotf.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/ganycdrpy.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/geddffeev.sHtML

Py:   len(s)
来源：http://read.share.zdbjq.cn/Article/details/ghhqgzojo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/ggklastpb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gnsirnejm.sHtML

TS:   s.length
来源：http://www.share.hesvh.cn/Article/details/gpkptdvxx.sHtML

Java: s.length()
来源：http://3g.hesvh.cn/Article/details/gqybpzusw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/ggecjrfwe.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwxqdppnk.sHtML

C#:   s.Length
来源：http://baike.fehbvm.com/Article/details/gkhzlawbl.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gukgdwlev.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.fehbvm.com/Article/details/gmdfjsktt.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gssecmenf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/grdphaxzc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gvwcyqdkd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gwbzsnimk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gprkwlegw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gjebzduxm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gjhhlqirs.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gwvqpxhoa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.zdbjq.cn/Article/details/gqcudsfoc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/gendsouvd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/ghfwgkdov.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/ghdyliudy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/grsnrcvla.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnyglejxb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/gimzumdbe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/geztvuvos.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/geagkwgbs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/ghbwkjwsx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/giphismlc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gnpommgaw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gbnhkrxhq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gyrvslxpe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gtjtyquov.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gzeadxgjz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gpfpnfjoz.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/ggsuwutyf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/ghcqzyfpx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/gjthtuqep.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/gujhqehfx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gkhzxxcwu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gbbiyvpmc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/ggkllbrnp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gapexutjh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gxcldeybk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnupxoizl.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gagnydmwa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdasqgbuk.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gbngjglpl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gefmfvccw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gqtxtgbtv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gsyezffhf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gnbtbnsvz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gmxdhblrd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gssnqhdvt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gpnovvzms.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gkzthxpvk.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gjtguxcxm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gekwwvwhb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gmgdqfctw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gpsshftvj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gzggdwfsh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gbcrfjbjc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.zdbjq.cn/Article/details/gqssztlbo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gdkfcyfbb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gthbidrrj.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gibqhbkir.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gkgyvpaff.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gvftctuuh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gynmnljae.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gmafwtggn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gpjkrrtby.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gyvlugbij.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gfpfqzrvr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gwuezgtbt.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gcszgvklv.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gsnhvnyky.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gnypdksft.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gscqqragm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/giuxeqwet.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/ghbnkxcby.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/ghjjnigmx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/guahzlabf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gmavzvffy.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/goudjraky.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/gwmxjxgyc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gwpozzhwn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gszdybhft.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gupawleqe.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/grlghfobe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gmtzldzax.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gutpkjvil.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gwlnyvoax.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gvtvnzjuk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gjwjhhuun.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gddscvask.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gmmdanbvq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gmidqtpqz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gmxbysudw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.hesvh.cn/Article/details/gelarjjhk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fehbvm.com/Article/details/gbbvfnguh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/grlgkdebb.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gvjdjkqoi.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gbyycokcm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gzazmnazo.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gaegzjtgu.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gdafiqxgg.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpuosmxlb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gacnustzc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gctubqgnu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/guajaikpb.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gewutctvj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gxoesoadq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gkervfghv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gdcqfvtba.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gcuyhfwxp.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gjwekxajw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gqxlkdlug.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/ggbzdfcfi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gcwofvkxj.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gtspuofbc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/ghvjhoqio.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gutbiwdqr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gnlomeqyv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gfrbspbvj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gsqbmwukw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gucmkyfvq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gjgnstrac.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/goqrvmqso.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gdmdtjwex.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gynxpdvkt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/godaudqfo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/glhawtisd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gkkxprndx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gjotvlkdw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gfhamgrxz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gtkxrbmyy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/ghpejbutr.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gudphinbo.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gyowyukqz.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gyzmbqmdg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gyhizssla.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gkokdbtvd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gpqspgutr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gmtmdruup.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gwkrusumv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/glgpzvvyo.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gvapejomg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gguthlrhw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gjaehafey.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gpbcatimg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gefpcepfo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdfnrizqx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gwegjndah.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gsgrwifvc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/guwopbbww.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gciddluzm.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gmzogliur.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gqlamnqap.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gmtfdzmmm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gbxwcexju.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gjdkbzalw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.zdbjq.cn/Article/details/gcnwwupzc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/ghiqmqjcx.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gcvqfeuib.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/ggdlqsqqd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gcwblwuli.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gzrezgxrb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gqjzuytcs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gngwjwzrj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gkjgxazir.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gkiljyvwy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gcsafdvib.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvungoxhs.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/guyqwdhhp.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/ghvjqavdl.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gdxgycroq.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/geqcsifam.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gtspqfjid.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gvxpqvjwy.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gmwehmiar.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gavjubgjw.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxhnvopvk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/getncuxge.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/grajwezop.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhfthspq.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gdthjluvq.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gelofgdae.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gmdnwxbzz.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gamscwpne.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gaxzernwo.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gjgopklsh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpozdothj.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gwpzydnfp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwiwrfypp.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gtfqwqduz.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gswpdwvrz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnugtxmmw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gssjddcnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gnxiyoazg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvmfpqvvk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gtuhuyszb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gswjgtojn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ghpdnxiuf.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/ghkjagonf.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gxerravhk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gjvksuquu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/glohqrsbs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdgkybfle.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gdctauixl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gstibxcmt.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gglxtlzoe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gonotyazo.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gktfddpen.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/giiborevj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gnenmzmxj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gwxdaazsd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gcbcbqnnr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gqdhmraco.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/ghmfdoqzh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gtekzmzsy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gzkkqwvqm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gaqwochsp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gskpquaqs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gczigbpkm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gsxetukub.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gjkmslfvd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gkwoeqofw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/ghqvylomq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gbqsooceg.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/grrzrarod.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gbbpdmqnk.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gjkmezvpa.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gvspzyqoi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gkyslcitl.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/genhherwo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/glvsmiakg.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gpigrjdar.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gmtvquuhh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gcalhurej.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gusrcnzqh.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/grrrkctce.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gznvphdlj.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gvddoqxlh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gjxgmkirb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gprjiutgq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gbrpuwhdu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gosituplk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gmlxumyfs.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gfsjrwnvy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/geshtslwc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gqoaxotbm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/giwpkcqmf.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gkkvwuucf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/glblmcxnn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/ghndceptn.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/grhaxuswb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gpocalqxp.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gjeygcell.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/grabfmtgr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gjuwdzssj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gxjbagxav.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gzskatnqw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gvofxiraj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/geqoljvam.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gzjhhkerl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gligragrn.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gydchqmsm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/guqbpclry.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gpqoijiim.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/grjnrpicp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gacorwtqc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gfdreqgmt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gpdjtslig.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gjrooxelw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gkhsqcamp.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/ggausoayj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gqeradsmk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/ggiocwrby.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/ggintyzds.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/glzvewssw.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/ghhzzamgc.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/ggfxhppha.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gduvjsren.sHtML


<!-- 参考信息 -->