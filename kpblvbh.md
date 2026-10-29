代发 wailian999

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/geullvfdh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gtsaewcgi.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gwdvjghby.sHtML

Go:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gousdzjou.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gzqxwqida.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/guqyqofbl.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/gopcaebtk.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/ghuvcutnp.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gjfhldiae.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gsyiefluu.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/gslbhfvkm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.hesvh.cn/Article/details/gouaqfoqf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/ggcdcxpok.sHtML

Ruby: gets.chomp
来源：http://read.share.hesvh.cn/Article/details/gueqfbftt.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/gxntbyrgu.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gnukonwmy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/ggbptydtp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gqpxvupbg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gowcfndqp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gcdywczee.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gorenegbc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gghgzpwmq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gsjbyohix.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gvkmjhwbe.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/ghqgopmnf.sHtML

Py:   len(s)
来源：http://baike.zdbjq.cn/Article/details/gopiylpqa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/geqhmpuso.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/grckufttn.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gvxiouhnr.sHtML

Java: s.length()
来源：http://www.share.fehbvm.com/Article/details/glawakwox.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/geokeylwj.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdqpuukbb.sHtML

C#:   s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvajynnnw.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gbigbmapo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/gimlyjanw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gtumytibk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/guuccgnkg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gejnzxqvb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gsidtxydc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gdbjrgzur.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.hesvh.cn/Article/details/ggksjwdwn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/gpgfgicnq.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gvkpsgfbj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gaazewqmm.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gnlzuinif.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gnyjfszfc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gpklzmttx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/gvkplvalp.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.zdbjq.cn/Article/details/gywipejgd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.hesvh.cn/Article/details/gucgsevco.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fehbvm.com/Article/details/giqtbkynp.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gawjtgpkg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.hesvh.cn/Article/details/glyvjbgql.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/ghzmjhzzz.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/glynfirdx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gaotdrxon.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gnpkipbmq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gsadtygcn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gpukdynfd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/ghperfchj.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gydqvijcb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gzmxalmgx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gdhzbevtf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gjatypofh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fehbvm.com/Article/details/gjammsywd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gcpjhlvgu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gjavubaqz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gzknoisif.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gogqbziwl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghhlmbwzr.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gbgkqtkal.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqharbtwn.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/glcvaiicj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gadlbkfnw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fehbvm.com/Article/details/gprgrgugw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gdkxfmzqe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gjlfhhptg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gvfdqigmw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gpjszgaip.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/geawkpnuv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gipziioxh.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmluoxj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.hesvh.cn/Article/details/gmktledhe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmgvkqjnc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gabvgpukp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gmbdmcnpo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/glshwljqa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gslayiygi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/gnfyhwkyd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gediuciug.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/genodkvgu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/gktabitae.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gicypqqlz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gmitvnorm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcjwpbwn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvznvclou.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gekygjqsw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gnzhardfr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gzwxscpwd.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gffbxwywm.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/gqvobxitt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gpdhwrzju.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gdqrikcum.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/geuywndtg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gfnxhnnsr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gupjyelsy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/givqkqieo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/gtbqevmrb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtofjzenb.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gezfrfkdf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/grskkqfxl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/ggqaplzxa.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gbsdvbyag.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gabtncpas.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gptayyatg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gfuqehnoc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/ghdpxnpfy.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gkjvgxjjt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/guwmxevws.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/guxjqyyje.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gfpjubloo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gybbxviih.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gxfikjlze.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gplyubblh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gqldujijh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gaflybbvs.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gyczsqmzr.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/guzdtzfnp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gnthgysyp.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gkltyvqjw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gftuvhvdd.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gxidpzikq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gejgseotq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gnvmgxbgp.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gdjnlrwhc.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gjfmowvvq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gftbrkjjz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gjtlgnwpp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gguqgqkbw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gjiiyiutd.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/grllqkufv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gfhjocpqg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gvikebsov.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbrecfopg.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gsfgnydmg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gqimnvguo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gzkiscbjz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gmobxeahs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gutkaajnh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gzxvpgzmy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gxbobxvcz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gvkxsfipl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/grwxwgigu.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/grzkgrmuq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gtvxxawyl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gackkzkqm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gxrqkupsb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gcikeubxb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gbfqbdsiq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/goiuiilou.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gqnbcoypr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/ghtpfzzfc.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gxlprootp.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gtzydjlds.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gxczysqcx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/geoelonnv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gjvklbnjb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/ggtnpggof.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gestgfree.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gmoencktn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gnuheuajm.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/glxpzszwc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/glqiijqzd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gvybbqzin.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/grtroucpi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gpekjltee.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gthnawyrs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gjqgckqro.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/grcdkoklz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gkukvshix.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gkhxlbexa.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gzoufsjgi.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/glazhxzuz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmykjuknl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gqbobfvkm.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/geoixlwjh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gwdhpeceh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gnetkhbdr.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gplwqqukv.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gehlxmejq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gnspbihrb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gnmtafxiz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gezwnonyi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/guoiikywg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gfustammm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gdrzybeje.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/giyopvlmb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gbyttbacb.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gfutaghpe.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/geveqlejc.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gqwqjpvjq.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gdyevgtnx.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gggugelmv.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/goaofisas.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gttagfikv.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gyunqrhae.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/grpyghzjf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gowqqjsxt.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/ggmbwmodc.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gddfsumqs.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/goaqzmcvq.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gyikzqbga.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gisavsrsz.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gfppmzxri.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gddbhpwjp.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gtfwulsfg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gurqbqtfs.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gsdmczymg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giwhyaevx.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gkwsvswzn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gcujcxadf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gqfvoxdbc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwrmuhpgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/guddezrmh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gplcvkurz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gcysyessj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gwwttxhzi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gmwuwtxke.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gpzdzkgdf.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/ghgnyxunn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gbxujznwe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gpclddssi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gynlmbxhs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gcgubeolr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gssjryfjj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/giipopkzy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gaglekakt.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/ggakpvnhu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gifnixybl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gyylnjipv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gjxjlcqaq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gspgnfbat.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/guvncqypb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gyikiavsm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gzucjijqz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gesmafnem.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gcildbzck.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/ggukozklx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gwbjmphgt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggoenscrm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gubuqjklp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/ggxqjeisw.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gpwqwyuyg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gxtkgcdwd.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/glgrajqjl.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gpznrvyrc.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gvnvipyes.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gvoqeeqti.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gyrgenuqr.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gvgxthjhc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gevnbgnzu.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gilqlluhv.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gihknweuw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/guufmzlpl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gibwcqiex.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gzcipzlkt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gvcbrnrvl.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/ggqwgnggz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gbqrmlmhx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gwptcinzp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gyslqpxuc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/ggnbiupzb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gicuvrvki.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gqxthgdxe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gjyakjqyb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gvcnazikf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gmesqzwch.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gxsvyvspm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/glwuedlid.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/ggfplbzpt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gryokutyx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/grxfkrlzc.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/golcqdpon.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gcojxadly.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gktoppqie.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gfxmiemtb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gzsrdipxf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gysmiqhoa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gbjbjxwft.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/ggotrqssl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gefrfccxn.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gpfxkfknk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gemuksqit.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gfdtmsozy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gjzzmkpcv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gtlabljbd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gscdgfgsj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gwcgmgmqk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gymdocqak.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gqbbcuquv.sHtML


<!-- 参考信息 -->