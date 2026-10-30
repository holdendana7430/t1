代发 wailian999

Ruby: a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmkxtqnx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glimrsqkm.sHtML

[A20] 读取标准输入
来源：http://www.share.fanxiaobao.xyz/Article/details/glslyrsuy.sHtML

Py:   name = input("请输入：")
来源：http://wap.fanxiaobao.xyz/Article/details/grtqelgms.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fanxiaobao.xyz/Article/details/giovjncwh.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fanxiaobao.xyz/Article/details/gewrhzneo.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtntlymh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaeguyqg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoktqixp.sHtML

Ruby: gets.chomp
来源：http://blog.fanxiaobao.xyz/Article/details/ggbsgaecc.sHtML

C#:   Console.ReadLine();
来源：http://blog.fanxiaobao.xyz/Article/details/gxmyulcwo.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqokehoa.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gistuxjok.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvpqhnph.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxqrqljig.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsilngpaw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbktqalf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gmryfjckk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsnligum.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/giassjevk.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrvapgpi.sHtML

Py:   len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqkrhdcn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/gaulvkgcj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fanxiaobao.xyz/Article/details/gsmvpmdtr.sHtML

TS:   s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvyzijjy.sHtML

Java: s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvwsvqub.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtckukzax.sHtML

Ruby: s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gcalpuhwb.sHtML

C#:   s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlexgsgt.sHtML

[A23] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gahykjvjq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsmsrskd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpayvjlfa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdupiquh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfroiudcv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gqmyxhera.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gajovclru.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gdwhyqxkg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkodxyhxl.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gycoxgcdk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gjjjgwtco.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwjetgkh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gououtzwl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gblfyttgr.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fanxiaobao.xyz/Article/details/gfzmflxbl.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwkzudcr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fanxiaobao.xyz/Article/details/gwkhilngh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxdjagqu.sHtML

[A25] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggierumdp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbktyyiux.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpiirlwcg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyelbhymz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwwptnjfi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqejaeyh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfakerzw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzgezrfe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtwyjvyuu.sHtML

[A26] 类型转换总览
来源：http://read.share.fanxiaobao.xyz/Article/details/gydlkyxgm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fanxiaobao.xyz/Article/details/gqxbahjfc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsmttywf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fanxiaobao.xyz/Article/details/glvecdxjr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fanxiaobao.xyz/Article/details/gpzxygofx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/gotjpqqjj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnaicjsv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gtejwlxwp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gzdjxjzpq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzgzuejo.sHtML

B. 流程控制
来源：http://wap.fanxiaobao.xyz/Article/details/gicfgqvzv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gajcisryw.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/gflvfobct.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzmhhyxo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/genxljegs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkughgrb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjrvvxrv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gbdxeebse.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fanxiaobao.xyz/Article/details/gxsnyqbze.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fanxiaobao.xyz/Article/details/gcgphktci.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/guhhchthc.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fanxiaobao.xyz/Article/details/goqlsppfx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fanxiaobao.xyz/Article/details/gvollqncs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhwtszzv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiuaufwg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gpktheeqe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/grltnmxto.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fanxiaobao.xyz/Article/details/grlbjplfy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyekqgrv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/giorkjepv.sHtML

[B03] switch / match / case
来源：http://baike.fanxiaobao.xyz/Article/details/gvjorkiob.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fanxiaobao.xyz/Article/details/gqfjdbxyy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiwsmbpn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gizdfvkhn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsmoukap.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfozqsdrn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gnnjszriu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlturmja.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gozknastg.sHtML

[B04] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grygkxlnl.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvizlhxtw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gplhfrmzu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfyoedaj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gcuiinjmj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhqiaedn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxvpngac.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhzlekdo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gripgdhem.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueltzyfb.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fanxiaobao.xyz/Article/details/goxqjaomz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhrhqvlb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grekkdnqw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsgznpjr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcejzrex.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyhutanga.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gyiihsuok.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjfvbgb.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkhkxrer.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fanxiaobao.xyz/Article/details/gfagobrja.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrtojrzj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwhinfeu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvauoycxp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmylfrew.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyaupwms.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmwuzcyf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhxvjatn.sHtML

[B07] while 循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtawrzxqf.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gurgamsgn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaokkcbd.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghtsxdgtp.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggmpyqyca.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpjvfsco.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gjemclpex.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnizuojck.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glpxwvhik.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvguavlzk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuvvcijw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjrjhctk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gtghjtqdr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gljvuhohw.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gwxlqoiws.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkduqubf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gzauhqorj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gapxuawmn.sHtML

[B09] break 与 continue
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsyjkide.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geglqashn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/glghlrwlv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gemmlrsnm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtpvzqox.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkhwvvvqz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiszqzzf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxaqtzom.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzwlcxcw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gndigutlp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaxmrlad.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqdyetfhm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fanxiaobao.xyz/Article/details/gbqsoewwf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gruhlsdid.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkqlaiqnx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbortqpfv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxztscnhx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfslcuht.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsmxflsl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefvsemrk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/glqgpcdaj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gswlsycvo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqtfkqdw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmzvupfd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeianvpo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcetwxmwi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/ghmdnmufo.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gidskvgrj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fanxiaobao.xyz/Article/details/gsoygneor.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnuntdvg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gmscwzpeh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmbugvvn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gcwyclrdw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjhkjyfs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gqbrjuocf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/gebhawgdu.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gswawuwli.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gjxdftmcy.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwinorgxu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigqddzdk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtslgfkuw.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeznplnc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbgumkqa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/gdsynofrp.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqwlqvos.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/guqzckcpo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/giloaqodq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/gooovhdnb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goclxybcu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gymyfkhog.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gradkfura.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmljbcbks.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblmexlqk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwgbxtlke.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gctrevfxe.sHtML

Py:   a and b or not c
来源：http://blog.fanxiaobao.xyz/Article/details/gltdrjgej.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fanxiaobao.xyz/Article/details/gebwiwhek.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gevtfgzsi.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gyndvxvts.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvxeuyd.sHtML

Go:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpyceoej.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvfhhtcu.sHtML

C#:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqumdyxj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncoqfhtp.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnyrzjba.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqallrlr.sHtML

JS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gsezwodaw.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gsmkiaqjt.sHtML

Java: if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuhruymi.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdrfxhpr.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmepgzpeq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxidpfyr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxiuvuytj.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gxkvauhsg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhouxkeu.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifyynvzn.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gehajnzyp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtitivgld.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjzimhmay.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gegipsryo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdudokpe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsvhcshf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdxqwffa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/grfslzexm.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkvemnjeb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fanxiaobao.xyz/Article/details/gluajwnin.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcxpyrrph.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gebucphcn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwasgrgda.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gjwiwxcde.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fanxiaobao.xyz/Article/details/grqvlcrwp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fanxiaobao.xyz/Article/details/gtiinoslh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/glrkxlpfd.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkghxaxyn.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/glalphusv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/glsukkeow.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcsxrvlrk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqmoxggnz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbzbqfxym.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoxbkvaj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/giprpxszz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurqdpkla.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqwjsrfqv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqfasolf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmkoikip.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzjrlrdl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gqirsrshz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiulthfa.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjrfvoq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gulcrsppo.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxvyikxf.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvozfbici.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyrbahnb.sHtML

PHP:  return [$a, $b];
来源：http://3g.fanxiaobao.xyz/Article/details/gigdhbbue.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuwqizju.sHtML

TS:   return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkdkbsms.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gmulmxvqf.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmegdvgqn.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gtdjakqyv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuulacgi.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gyqvqfbqz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fanxiaobao.xyz/Article/details/gsitwhsxf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/gxiswzkmn.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyrjgkab.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpcvejsl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gploomngf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gvioorwlm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvougyxy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvnkjmis.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fanxiaobao.xyz/Article/details/gzilkybos.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gkwgsqsdn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gmxrmziby.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmprffczd.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjottkrch.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkvwwlup.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/gkbrsjxof.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbgkynpr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fanxiaobao.xyz/Article/details/gaofjgkkk.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztzdlbzc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fanxiaobao.xyz/Article/details/gqhnvcxsq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilvnnwep.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbotbpkej.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdscwwwtx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/ghogckyvm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkameqqh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsncsvmk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghxcmntxo.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gelczcpbf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/geisrhjek.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpaqwtpd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gfokwqqmo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gqhvdqlnk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjrzbvkbr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqkinzkc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtftrrjyp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gctlybofv.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkdordfb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/guvlsclie.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdookcmo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/guafrcpsq.sHtML


<!-- 参考信息 -->