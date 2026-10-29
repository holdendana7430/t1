代发 wailian999

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gahpaidnt.sHtML

[A19] 交换两个变量
来源：http://www.blog.fehbvm.com/Article/details/gmmqmzwvg.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gljtedzjh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.hesvh.cn/Article/details/gollmrsbo.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/glgukxzbg.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gxulgicxj.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gchjyyevs.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gjulzbpyr.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gktcmoqff.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gordehrjt.sHtML

[A20] 读取标准输入
来源：http://baike.hesvh.cn/Article/details/gdugpqodu.sHtML

Py:   name = input("请输入：")
来源：http://blog.fehbvm.com/Article/details/genznhtoh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/gsvnhdzlo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fehbvm.com/Article/details/gwezqpujh.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gorfkyxfk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.zdbjq.cn/Article/details/ginsqpuzr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.hesvh.cn/Article/details/gfivyusmg.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gqeqbvtct.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gdwhabeiq.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gfrrkvdja.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gjxbwczeh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gajlevzub.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gijhjtgde.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/grybfhroh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmujzyo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gfffdwaqx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gwrvaqfjo.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/giyanvlcy.sHtML

[A22] 获取字符串长度
来源：http://wap.fehbvm.com/Article/details/gjkfprbvt.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwbeivye.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/gzsxsxtxw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/glloiegqj.sHtML

TS:   s.length
来源：http://blog.hesvh.cn/Article/details/grpjjwuys.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gunuoqdpq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.hesvh.cn/Article/details/gbnwdeiir.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gasfizwwc.sHtML

C#:   s.Length
来源：http://blog.hesvh.cn/Article/details/guzvmksmt.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gipyylfab.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.hesvh.cn/Article/details/grqoipboh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gpoossklp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gdlsmssqc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gxijpnwuk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/guikttjnx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gampwiksj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.hesvh.cn/Article/details/goafwekwk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gygeqhpeg.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gsyxdcqww.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/gmqmopiuo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbmgujpd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/grpqiebon.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gcjcvrxtt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gpllurpfg.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gijgkxcvd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/gqxwuplah.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/gclvwpjid.sHtML

[A25] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gzvirofun.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/gyxxvgusd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gwfxtddwo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gunjvwcou.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gmxdglaqs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/giawoafgt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gdoilobys.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.zdbjq.cn/Article/details/gvypohtiw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gulbnakyi.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gcyvxjfkh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fehbvm.com/Article/details/giitqykyc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gmramzcvv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gemxzkxct.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fehbvm.com/Article/details/grogpqtcy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gfeitoiox.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/genxgjkaw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/gdizyqebw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gzoivfevz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwxbzowzm.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/grlpwpmka.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdpwolsih.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fehbvm.com/Article/details/guzihdyzu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gonvyxrqv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.zdbjq.cn/Article/details/gcdkelceg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gmqyqkuag.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gqmqnicpx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gcngdhzeo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/gwpoctykn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gdchfgida.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gosdcjgsg.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gqakmsswc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/ghfnriqin.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/ggdsqbtaq.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gvlvgzaor.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gzadzwwpp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gkmydsbql.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gkriacell.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gdxfeyffp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gegmmwaiw.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gosnrbzli.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gdfjlbikj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gswsoxvpb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/ghatppxio.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gtgjvuref.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gzcqiggxn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/ghrgysoqx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gywwhrzlu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gljrklymf.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/grkmfgfnn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.zdbjq.cn/Article/details/gofdujcjt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdcqmhwpe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gmnjxndyk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gdrtwnsli.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/gewbqhqyw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/ghjxqfhzv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/getmdklog.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/goskxyqcw.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gfgsqpdxu.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/grlphdoqi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gwjxcsdpc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/gxjhgwugt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/glnyxuhqc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.fehbvm.com/Article/details/gjrhbjiff.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/ggfrujext.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/ghlomgzim.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gsuidvknh.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gepftenlz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gcbzxbfqf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fehbvm.com/Article/details/gdwyufcwj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gcgfsqoom.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gpjuqtuxr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/grgotxwdw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gxkhdkqmx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gwojujgqp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gjqdiondl.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gmsjxpwcg.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gcmomholp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/giqnfrntu.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gxublddlo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gdnfyclib.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/glicutloh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gqfhknzgw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gyqincyvy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gwcqxcbfw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gqjseuraz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gmoyidiey.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvjrielgb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gqzgvhles.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gphrivkzg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gnwpudosh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gxigonmme.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gzxhgvaap.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gpibwfrew.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gizqexejo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gdzuasawi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gokyeiwgd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gjinrylhn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gjiqpeclo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gbbqrabgf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/grfrhgdaa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gdrsrnavr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxsqqvny.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gryypydbe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gjfujmqvc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggwqxwbwo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gjxwnqmmz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/ganglprqx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gjdkkdpwg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gdvghezob.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/graltwflq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gcsqysmez.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gbetxudys.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gcwlyjttv.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gfhbkkwjp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/ggkhgrwmd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gubgqoakq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gfeihvbnk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gzbuuzkux.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gkxtdacos.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/ghgaiwwch.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/ggwoiolwm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gwwpogvvb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gpkfsgyds.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/ghkudjccu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/goihnrvdf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gwrndxudi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gsczyovqx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gmnfhbwhd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gydczdrut.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gnmswapkm.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gvenexvpd.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gsqyirevv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwvxygdpb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gpqaqghwe.sHtML

Java: x instanceof Number
来源：http://mobile.fehbvm.com/Article/details/graicivcc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gqughsndn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gzwzwmnui.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gsicggqnp.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gxcxcmayz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gggtnocvi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gnhevuntb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gajlliajv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gebhhmjcz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gruovpszj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtowpcdky.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/ghzougdvm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/ghhtlgzem.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/grfrdtxjq.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gnxtgrkjk.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gpmzjdhth.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gkzmfcjzh.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/guomnzvan.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmkxkzksk.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gvydwkpiz.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxurkzlzi.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gjrullyra.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gytdwadwb.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gkclufbpt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvytpfky.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gkmumqdyh.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gazjrzxoy.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/grhkoltjk.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gidkzfuua.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gwvonuguw.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gaqtkbyez.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghcldplnl.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/ggjekaohw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzxeeyzch.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gmuvkhkct.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/giyrwynzm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gvrhpjewb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gketafbnv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpgseeoeh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gljjokjlj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gijkglcuw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gyrbkiguy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gszrpktkx.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gmdsokcwc.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/geblcufdh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gtpkydicl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gkxjbsziw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmaivwczs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gazxdsnxx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gnsagmnwd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwiiuer.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gmuslfksa.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gckmthhpg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gvemxwgkg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gcrmxykuk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gsqxlbtac.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gmvqzqpjt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghtvbkqij.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gnslkhdyi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gvtsqkbki.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gellvkjlb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gmdtcqqgh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gnokxlhsh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/grmehdqfo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvfmerghk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gttczzlsk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/grtgubhnx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gmgiwhqrq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gkhsqhfbu.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gtcdyshgn.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gjsflpinw.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/ggekeskne.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gsgeohebp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/galdrucbs.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gmeulqsip.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/ghropcbty.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrkgmsf.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gdloflpkt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gcicoteiy.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gbgivpgef.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gcmxypesh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gsrbazqbm.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzerlqykv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gdnykpmzw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gvtpykwae.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gjbbczgwt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gmuxhljft.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/ghnecwilo.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gqjirbtzt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gteagfiyy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gndpzeatj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gweejyktk.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/glpbrflfv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/ggijruncp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gqbswjuxd.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gcpiuqpta.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gyvwglygh.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gsdokuphu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gmldvpxor.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gdimwqumr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkyjenk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gjnsuiygi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/ggaofhkjh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gjcqrlsds.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gyoumfjuk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/goewqslrf.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvivhtj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gnubygppx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gwdoarynp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gupbwenbk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gxjxbfsni.sHtML


<!-- 参考信息 -->