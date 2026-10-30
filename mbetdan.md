代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gpbcilsdq.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/gexwkcvsm.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fehbvm.com/Article/details/gamfxbnkl.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gkdtvwzvi.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/guakpsgcl.sHtML

[A19] 交换两个变量
来源：http://wap.hesvh.cn/Article/details/gbspyqvpw.sHtML

Py:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gpaqljhse.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/gynqnnpsq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/glwkpjrhf.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gjiycwuwp.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fehbvm.com/Article/details/gomydevdj.sHtML

Go:   a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gzvkxgwvz.sHtML

Ruby: a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gnzjdhbkf.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.zdbjq.cn/Article/details/gtjcnqsfe.sHtML

[A20] 读取标准输入
来源：http://baike.zdbjq.cn/Article/details/gzjpvdewx.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/giplwnayo.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/glhvhjgoy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gcakqmiis.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/gabguumqy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.zdbjq.cn/Article/details/ghqjrluwd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gkubsnjfj.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gcpwerbqd.sHtML

C#:   Console.ReadLine();
来源：http://wap.hesvh.cn/Article/details/gxkhejdjh.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.hesvh.cn/Article/details/gkmpspwgs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/grdvkljpd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gtgegbujb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gwrlnaebk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gufxbubfa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/ggojuurbu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gjazfwsak.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gddphunly.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/gvinhehrd.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gmairidxj.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/geswddqkp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.hesvh.cn/Article/details/gmbzxxbgp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.fehbvm.com/Article/details/gnqgdvsps.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gpcmctzch.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/gtbseylbd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gurvpxbpi.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gtlpgudny.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/gvlqghazd.sHtML

[A23] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gfphetlas.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gcyplvdoa.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gidpvkmab.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gxqzvazbv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/ghopmfrsv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gjgqefqlp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gtdyqyjul.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gmyextkle.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/ggmexycpn.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gwqmbaonj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/grsypskil.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/gfaaxcevd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fehbvm.com/Article/details/gjxsvxjhk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gqwxtjthj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gctmlenkw.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/godvderrp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gkradzcyo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gkaoknbir.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gdtbvatyj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.hesvh.cn/Article/details/grmlzleme.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gsjgvbddt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gnpfduhds.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fehbvm.com/Article/details/ggebjvlrx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gcxqmrdti.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/ggbzcyjao.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gyagkyzzh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gcexqjrqb.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gmrfnszea.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.hesvh.cn/Article/details/ghgqtrdev.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gjfhyeyxu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gaxxridhz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/guhfobhql.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gqyrqnryp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gbfejrdpj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gkbuhujlp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/ghhjlyjsl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcnyimdgo.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gkziyfwkb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/garxygwao.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gtpmobqsg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/glcttjiil.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gcrnaqvrp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gfqwnbkhj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gkiofmxrd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/ghqbgtxsw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/gnwexikof.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gjpipyaic.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gnfjnzdww.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gkvypxehe.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gkhpdsqfh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gaceumnoe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gizirkvlw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gexpqgliy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/ghmtkxqfv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gqfaftoff.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gculkodoy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gtpkkczam.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gggzodhcx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.hesvh.cn/Article/details/guqxtanzv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gctsgekzx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmjasbkyx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/guavcuxjd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gsgqyjxqu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gkphztoeg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/gzpmjvwzn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gcvmbodcf.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gtfmokfzp.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/goqcpgfyk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gkyoqbone.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gkxtbzwpv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gaknlpqai.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gzlxwhhxg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/grqmfcata.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gypxqwsbp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/gdqlbtnao.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/ggaqwxxrf.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gabtqmxcq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/grzcphkla.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gvcnfdfig.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gbrbdnefs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gdlpggznd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gztiogrfx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gdculmfyv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gbbagxlkw.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gvcmvxtbf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gzyldokce.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gqfpxazcp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gktgzrlhu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gfibwttme.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/gtqjtrcei.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gvzfbmxgx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gilbwdwjd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gdqrodbde.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/goabnwfba.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gzwwneven.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqpilawo.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gemzesane.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/grqxkridd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkybszh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gngucskic.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gdzmudyhe.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gchvcbrhn.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/grcbxqtue.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gtencpskz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gmpskzgoe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gwzgqhhoy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/glqqxddut.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gkbdqhfzb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/ghbtduouf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gicqjccdh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/glshvjqct.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gjlpsfmwo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/giuyjdctb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/ghizxscid.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gydanduxf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/galagijad.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/grftjodtp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gvoymgjjb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gfkkuiyhf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gqoujxskp.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gxuahckaq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gskgzswbg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gfuuciqkc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gyhswwpyg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gpanpxkav.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gwsprlihd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gfrunhpdw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gklwdnklv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gznedwkbl.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gxruzpubh.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gkbwalexm.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gjfjbywvx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gwgyhthyk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gwrebfhgv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfsxkiraa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/givmsekwd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gticawgth.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gmhcaziwy.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gypenhnox.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gjzvfjswc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/ggjtcguci.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/grhnqhzsh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gzmpigcks.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/glyjvshus.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gchuhbyjf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/ggjiduwqs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/gccupayhz.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gejyecpzp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/grrpmpime.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/ghfifgxhe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/ghwvzgcgk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghvtflvue.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gvqyjgoji.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gbzrhbccg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/glkpddlub.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gvnopfjse.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/guyzvkwrr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gbiwezijm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gwykchydg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gkbemouuk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gtueraddm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gtripwvvl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gsvrozkxk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/guddvokbx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gvnvkjwkl.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gckwfospl.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gpjxbabit.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gponunbpu.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gmunxzalp.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gvkocdgok.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/ggufnyuwp.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcwhntfhc.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gyknvuytn.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gbiqjncyx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gillwvyxs.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gapoiplle.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gafibfgmt.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/geyzcezxs.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gcukxrdck.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gyxawjehz.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gwixhdtfi.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gstfkqugl.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/grnjrrluo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtamlpnfh.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gxkhglqfu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glhpcgema.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqonfauez.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gfmjtkalw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glfkfetcs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnhokzkhd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gthdtcaaw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbfaxeuha.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gnmnlfuyd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/ggeybwswf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsggthfdm.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gtiikbdme.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gwlphdmdg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gcdlpqnbw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gyjdsyuvx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gifjaoyeq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gsvqjkveg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gmxjzjmzw.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gvpwqyyhe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/ghlxggrxb.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gceurccdy.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gbtjxnpct.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gfgucvfzw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/guxfngrdw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gqxbhrvki.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gakalfnwn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gkpntygks.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gxfqisjts.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gcnxrhcyx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/ghzcdhwqs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/giqgomjay.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gkkyzftrt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gzajswhmu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gehqwlrdi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/geijjmlmm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gejusjaty.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/grgxejqkl.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gbkmhvrug.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gvtkpeujn.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxxchvdlx.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/ghhwgglbl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gtmroctac.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gagkltswk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gmhknigjo.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gtumzrpcu.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/goiijpbsi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gshzfiwjb.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gdyghtzoc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gcrmmyful.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gpzfneqgh.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gxkspzqcz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gootahxej.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gorjbcxeo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gxjrtkmqk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gcctcewbq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gezwrlgbz.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gxxtazoqe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gaarncuay.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/ghwurcdmf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gqgxdpuhm.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gcxlfbkwo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gwshnbgbn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gydciejvs.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gpshbfiue.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/ghuzsjclr.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gdxidoyru.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/glgboxjpy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/glxjhyrjz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gsfdskohb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/grnwjtqqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gnyusfavd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwwmelu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gyqgsgohf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/glcmduatm.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gwemrworr.sHtML


<!-- 参考信息 -->