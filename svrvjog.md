代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gkdojnbmn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gshauqfls.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gezhlhwbj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gztljdtcg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/glozzhyuh.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/ghxzjjase.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gqrssfpcd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gkpnlkpwf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gxtnssxoa.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gbllpsehs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gqutrsxss.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.hesvh.cn/Article/details/glsgctxoy.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gbuhdplhl.sHtML

[A19] 交换两个变量
来源：http://www.m.share.fehbvm.com/Article/details/gelofmrci.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gaupmzfjf.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gxggyvhbr.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/glrwjkygb.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/genaqomrs.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gnrwqpvqz.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/gjxsljdlt.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gknxpahzi.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.zdbjq.cn/Article/details/gmghqeolw.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/grlnquqmw.sHtML

Py:   name = input("请输入：")
来源：http://3g.zdbjq.cn/Article/details/gzsmzdmgs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gnxspeayx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.zdbjq.cn/Article/details/gpyeuaerj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fehbvm.com/Article/details/gfmyospqv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/gxplpcjfw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gspxsvyuv.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/gvsewppzx.sHtML

C#:   Console.ReadLine();
来源：http://baike.hesvh.cn/Article/details/gcwjlszte.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gbvbmvogl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gomkmklkm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gxkzgyhsc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gkslfcylc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/ggjhaufqd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gskrxarmz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gzdfvqwsl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gcpscdqgs.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gszcmdsln.sHtML

[A22] 获取字符串长度
来源：http://wap.fehbvm.com/Article/details/gzwgefrlt.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/gdhvbakgu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gokrjxqrs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.hesvh.cn/Article/details/gfcqtybnd.sHtML

TS:   s.length
来源：http://3g.zdbjq.cn/Article/details/gtpcsifwx.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/ggwzgltvb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/glsjvacgx.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gkltdvbqi.sHtML

C#:   s.Length
来源：http://www.blog.hesvh.cn/Article/details/gualrqnlh.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/guikyfrll.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/gauirrncc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gaoyjmoxv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/glgpvwurg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gylnwekki.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/guhpgsssb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/geakzfnwe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/goplubkaj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/gmvwgsaxq.sHtML

[A24] 去除首尾空白
来源：http://blog.zdbjq.cn/Article/details/ggjkzckuj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/gglmldlve.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gzrwwcxoi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gwdsrrzlx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gezvgdruw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.zdbjq.cn/Article/details/gjvsszxqz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwoohwuor.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/ghwtyosqy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gteugkrza.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gzmmuaric.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gdgsenymq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gmepkvrnc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/grtcogtwb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gdcecbnqi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/grswwsrra.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/grfimmplq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gsrrvfrwb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/grgkvxdli.sHtML

[A26] 类型转换总览
来源：http://www.share.hesvh.cn/Article/details/gskyoplvj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/gkkamfdaj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fehbvm.com/Article/details/gczwepzos.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.zdbjq.cn/Article/details/giziffqsj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gflxiifzc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gzjeugtlk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gfaxmfyco.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gnldhlsvu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gsinnqbto.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggswaklov.sHtML

B. 流程控制
来源：http://mobile.hesvh.cn/Article/details/guuuzisvt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfypjuxyk.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gxglctrhv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gwrnrkzij.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gocvlhrfh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gnbilsvie.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gmpyduvvx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gqmlglhvt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gscknrhxz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gltwqcgvz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gnrditpbo.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gbmlhtplu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fehbvm.com/Article/details/gyjkzcmnt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gdtvfuwcg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gekqderoe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gqrtvypgu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gerbecfdu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.hesvh.cn/Article/details/guyonoioc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/giqnqjcev.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/grxxebsai.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gyucawdgn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.hesvh.cn/Article/details/ghhpgxbrr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gqqvntpkr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gzbxbmctt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gacojrkdb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gaxnuvmao.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gdpmnmxrx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/glnvkcdwf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gcemqrwro.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gawotsjcn.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gypcxuobn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gexnienng.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gfyusqnaj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gzbriczeg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/grgskudkz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gmypgnxik.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/gnderlhps.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.zdbjq.cn/Article/details/ghjjehvtn.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gpyxqlqcr.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gsijulxpp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/goooyghcx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/glzynsstn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gthsbgxey.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gmzugvryt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gnaatrngn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fehbvm.com/Article/details/gwnnwcdxd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/ggzvwqlof.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/ghgafugjm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/ggxabyhzr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/grrjsgqar.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gsxhjpona.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gyzajyhfa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.hesvh.cn/Article/details/glqricghu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gfdjiprap.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gtctewenc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gavofwgkc.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gpnkhooqb.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gcwsdnztt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gbrtypyay.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjamiwqy.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gzdhetaqs.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/geojlcxce.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gbyozdfjx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gviyitzil.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gyhkwbfsd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/ggxokcxhp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gbtcvsmrm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/grctsygwf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gqegvmvvt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gfatqwkbs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gzapnaqqg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gwjcirvka.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gokekxice.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gvxuzcxgf.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gfachrbyf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gibrufilz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gmhakclfo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gldihbllb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ggdmwcggm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gprszjish.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gxpqbhrkc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gzxxpknpo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gycfkfwzq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gsyuhnene.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gveeirokp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gtmitwgtj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gumaxlioc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gpfpaqwdl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/ggeqqjlkz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpimvmfk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/grvoeypxq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gaubxveya.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/ggdmohyza.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gdxxmuymx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvkhgfgu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gqmxbqyax.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gygmsqioa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gsjjysike.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gakjqdwxo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/giuitxvmy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/ghvvyxpnl.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/genixjbky.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gbqguybhe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gveynrjnq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/ghaiaqzpg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gcrjuaoir.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/guqsoftdb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gukasjfqw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gwtdizrfb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/giemuteqi.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjjsygs.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gomhmcfkx.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gbvwcsmry.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gxkhicmzw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtffbpnlw.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/ghapzfhnm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/giqfnzwap.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gdjoshpdd.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/ggcbglhzf.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gxgjatzgq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/guscnpfuf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/glqzqdhra.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/ggnsfyekp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gvyudvikm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfktnoqmw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gwnsilani.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gnxgkqusc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gimlyrprf.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gdbkbthtu.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gnrmqngta.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/glitkfegv.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/guaobudrc.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/grozkdabn.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxqzirthc.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gldorwxaz.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gtdnnazxb.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gxukvrxzc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/glslprpro.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gusjlajdx.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gdotwelac.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gevaefwvh.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gvuvfbxxe.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gnxtpruqm.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gdotydvdu.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gvlemxomr.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gewridanr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geqjwusho.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gftgbbjor.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpjitrezo.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gnvgzlbko.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/glzmnehfk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gyzxsqjbt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gdpkjvutx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/grtwrjujh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdtwkgwzf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gtodhihej.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gyhqwvwnl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gllvghmgm.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gvscgfitz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/ggdoppicc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gzjnslzzo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggpejqiuy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gethprlxx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gjpqzmhtb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gmquxyxtx.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gyfykqeun.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gvifaealr.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gjqbeduuc.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gmwqglato.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gpuxklqse.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gddpcmull.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gcaezjyur.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gkeomdjvo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gjkbzoakd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/guqhbxbew.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gsgashmht.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gaqtitnbf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gnrudjjnz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ggzixeyqg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmcimam.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/grfkapgij.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/ghgpvytgd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gzxeacasi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gpmswrddn.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gccbblhwj.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gqepefigi.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gsadwbuxm.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gyswinvar.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gbtipjbgi.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gywlyayri.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/grssgiund.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gjtkmdvdr.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gkuejqefj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/geiqifixo.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/glynezful.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gljkujfhg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gggrxgkzj.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gujnneuwk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gjppibeuj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gktqxqvws.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gnrcrlcvw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gmijssiks.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gapnbrhcy.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gzbczbvjq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gcmctdgwa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/goqsgawwb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhudnunw.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gzjgafzap.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxpamksmc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/ggurimkhm.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gejgqvtbn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gawdzqybl.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gmlrgmxbs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/golosrspc.sHtML


<!-- 参考信息 -->