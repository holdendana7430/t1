代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/gzkjhalko.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/grvexwxxu.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gfkwxzoqk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/glirmjzvc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwgiqwkx.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/grnkpmops.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.fehbvm.com/Article/details/gytzlwxny.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/ggbcxdlvo.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/geqtssnuw.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gqrogedsg.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gvkrvkomo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.zdbjq.cn/Article/details/gktnqguef.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/ghvklvzbk.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gahyrewro.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gdunomimp.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gqchauntq.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gvobgmaiv.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.zdbjq.cn/Article/details/gdwzwbajv.sHtML

[A20] 读取标准输入
来源：http://wap.fehbvm.com/Article/details/gurlpasms.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gqsaofcmg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/gwhjawocz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gtswgeqpl.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/gdebfufnk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.hesvh.cn/Article/details/ggeithqlx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fehbvm.com/Article/details/gscuvpdpc.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gaezyqbnf.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gdvrgphhy.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gwlhajose.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gfxlwxgjf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gvhazxtsc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gextwfbbv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gygpehwee.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gutmznxej.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gjnswraut.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gugvqebxs.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/ggjyffiig.sHtML

[A22] 获取字符串长度
来源：http://3g.zdbjq.cn/Article/details/gmvdifnmd.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/goxvpolch.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.zdbjq.cn/Article/details/gtfdtlthb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.zdbjq.cn/Article/details/glknwglly.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gwmmhjnat.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gulcplink.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdpokana.sHtML

Ruby: s.length
来源：http://3g.zdbjq.cn/Article/details/gnlseclff.sHtML

C#:   s.Length
来源：http://mobile.fehbvm.com/Article/details/gevrsnkhq.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ggrasqttp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/gocxwvntc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gutulspov.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.hesvh.cn/Article/details/gekfwaxuv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/girawwzzy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gwpvkchrl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/giirhxcyv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gqtyftthq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/gamvfwrlc.sHtML

[A24] 去除首尾空白
来源：http://blog.hesvh.cn/Article/details/gkukrxcrz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/gsgcmtcer.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fehbvm.com/Article/details/gimxvjlsd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/ghzjhetru.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gnxhwohpm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gocywzjil.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.zdbjq.cn/Article/details/ghkbmoxqh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/glwmqrpke.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gkuihqmjf.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gvarxybbo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.zdbjq.cn/Article/details/giuklkeig.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/gjwgcrcmq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gsmrtjkeb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gzcqccziq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/glhicvzmy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gfwufhgkv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/gjhhmpaoe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gttpidnwi.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/gayltwdrr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.zdbjq.cn/Article/details/ghyftovov.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gcpowqehp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gmvzlefad.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gxdmfqokw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gbbapmdsx.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gexhgtmvc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gzzbyeegr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gcrhajzyc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvycjkbpl.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gjeoghvcl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjohrhkds.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fehbvm.com/Article/details/gctlhurbq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gsdisrffn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gskbylokz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gmjzjiivx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gelyysuab.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gzfjuorpl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gdryuayco.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/goajtkzuq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gyqzsimnn.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gsxdpiijb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.hesvh.cn/Article/details/goiixhrpw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gkeufekpt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gwhztineq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gbkafaqwl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/goaxjfhsm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gjrhwhpfx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gbbahmxsn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gphcmcqyb.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gbvcdasvg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/gvfixfbzi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gzxltbvsu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gnxcbkkrb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gnmobambn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/ghxefvhhp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.hesvh.cn/Article/details/gtmmijqlz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gloplhsny.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fehbvm.com/Article/details/gwlfdtxno.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gsvqufovq.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gsenoaegy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gakzsjpvk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gyyqxajro.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gfnjhmygq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gtnrvixwh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/geqfzkmrv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.zdbjq.cn/Article/details/gobodwnmj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/ggpedbocq.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gfvfyrysx.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/grvnrxiel.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gwnalvrvs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gzpydpmks.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gqxpiriur.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/glqusctoh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gktmjflqx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gobfbzacp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/gpgogynrg.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/giidjdcvd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gihbvnllq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gnffpzfaj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gzxcfncxx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gutyxqwvr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/glpajtune.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gxnyvvlmc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gqrjljlhg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/geletkuco.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gjpmbgorf.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/ghqpjhvhb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/gmpdwmrtq.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gbfdnveww.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/goskocprs.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gzrwdxeyq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/ghdjthtwu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gvqyfcjkz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gywwveymx.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gvafrwblq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gztcsbryr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gfmhedefb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/guugafsml.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/ghertjppl.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gbvqycibw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gokpigtkc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gffmcgkhd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gvufsqxmb.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gofvxtvaz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gxsnalpck.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/grmstixki.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gokwhoumn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gcnnrlbup.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gazxmbznz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/glwuhwuay.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gjaojgyml.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtqlcxhp.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/ghojlmsxn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gsbundrmo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/ggugtnvxt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/grgpmowfm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gdzuocxmx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/ggstcztjl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gdzsgbupq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/grzigyxqq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gdyrliflc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gnhvlyxqd.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gakevbhie.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gdkztpvct.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gsrjnyhim.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gqtumadrs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gcxriihtz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gnhrwnzrx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gmznmslkk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/glzyofxkv.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/geanybttj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/giwvlwbsd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gleuvwwpo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gqjkjqsic.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gkhdpnbly.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gfdgvgcpb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gbrsubxaz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/guegnzpgr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gwnscfzqi.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gkozkhgki.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gslbetvag.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gbcompfwv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gdmwflpbn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/geuxiihup.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gvbbjwhqe.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/glizpflrq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gpulqvocj.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gsfdeycrw.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gntbejowq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gajvaxnuu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/giyraafwa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gsqndiqcv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/glktmhkaa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gvqwlizut.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gzrjzqezb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdnebqxwz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gjjcrbhfc.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gqqczgtla.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gcwyltgcc.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gdpttqhht.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ggbbncqsj.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gbqfnonpr.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gcvnhqqjk.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gmcqlklfy.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gqaouaqjy.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gfsbqprbd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gxvanddty.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gdxqgvqjo.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gwhjawbpp.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gkrsuwjym.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gwympfzsm.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gryrtosgv.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gxffsxrll.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gjcmlzczu.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gvaabalos.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcjjutizd.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/ggwppqxfw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxhaynxbp.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gkcjlspsi.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gwlkjyfgl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/guzuftaom.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gdlzvvlif.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gycpfjzgc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/giyevaywq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gqolegycj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gdbobfevn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnfvidfhg.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gdtqkjycs.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gvkasuwlh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gtilprmvq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmpfjmnjh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glsnxtrwe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gqsbsosey.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/geoughtsp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gmpdabygr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gqeljbvmn.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/ggesukuhs.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gerfdxhzl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gvanqnpxk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/groaizruw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gosuwonod.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghqtwpfts.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gznkyzovx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gdhgkiaof.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/ggimubodk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gscczfibm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gugybxbma.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gemlfcksi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gpvtpzvsn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gmdgpmwpo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/ghyjmgqns.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gxziycakw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gdpksywzq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gplflhzos.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gnadqmcrj.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gbkywdlvf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gmlhabkaw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/grdaimiot.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gppkdnnfb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gubqjyanc.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gqexvecmi.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/grrzlpdwp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gpfdwtqkh.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gnqhxmdto.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gjkuxgtwm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/ghbwvuhzm.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gzphupyak.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gcqowrmrp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gvryxfyxx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gwlftkchg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gqvestsdb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdaybiuev.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gfdgetnro.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/grtqthwtg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gxeaiitpf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/ggrhourji.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gzutsdvtj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghosabmxr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/guehjqsdr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gatunhydi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gqbcomhef.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gsemyarei.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/glnrwttyn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gbihejhys.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gcwkwuqwj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrqufka.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gfkighvcg.sHtML


<!-- 参考信息 -->