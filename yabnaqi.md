代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.hesvh.cn/Article/details/gkvmbzpzq.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gnrawdajy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fehbvm.com/Article/details/gldcvyguk.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gcbvvlafa.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.hesvh.cn/Article/details/gzsivwyiq.sHtML

[A19] 交换两个变量
来源：http://www.share.zdbjq.cn/Article/details/gchzlpnah.sHtML

Py:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gccljqlyw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.zdbjq.cn/Article/details/gmfbwcztm.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gxuitailc.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gapzzrtdm.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.hesvh.cn/Article/details/gldpersih.sHtML

Go:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gwcikeeny.sHtML

Ruby: a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/guayfhljw.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gcebuwyqf.sHtML

[A20] 读取标准输入
来源：http://www.blog.fehbvm.com/Article/details/gmoxwwtqy.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.hesvh.cn/Article/details/gfjpmvxdi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.zdbjq.cn/Article/details/gcfbykaod.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gsnhqpmht.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.zdbjq.cn/Article/details/gtxxbqgzt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.zdbjq.cn/Article/details/gdxbpxcto.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/gpdhuhtmh.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gvoyvkydd.sHtML

C#:   Console.ReadLine();
来源：http://m.share.hesvh.cn/Article/details/gfwutplpi.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fehbvm.com/Article/details/gdtnhrtqi.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/gzztwtzpi.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gjeratptv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gmzileohi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/ghuwusrvo.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gjgpigyww.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gfpkvijbo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gpoahlbhh.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gzgcgggop.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gcxfzslot.sHtML

Py:   len(s)
来源：http://www.share.fehbvm.com/Article/details/gohpkawct.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fehbvm.com/Article/details/gjhqbiuvc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.zdbjq.cn/Article/details/gpfctcibj.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gxwexpjze.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/gufilwdyu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/gctpejsew.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/gftosqhqx.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/ggtrnkzsq.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/ghogravdh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gqeyzsadh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fehbvm.com/Article/details/gkbobernt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gmkzxpqma.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fehbvm.com/Article/details/gqtrqzctz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gehsejhop.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.zdbjq.cn/Article/details/ggetfqgki.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/ggzwhpmrr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gqvlhjyxx.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gdnphpikt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gnpqvvcwg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gpelpnfqd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/goivegncr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gifcmwcae.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fehbvm.com/Article/details/gtajbhkfc.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gagcbvaik.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gckuswoot.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfabetvzw.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gjxvscdvu.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.hesvh.cn/Article/details/gsvpmdyhw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gmavddetr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/grzerprrk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gfyyyxnde.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gsuxbajsm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gxvnhiaaz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/gklavqktu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gugrcusou.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gsgliipen.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gmudrlmve.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.hesvh.cn/Article/details/gdbrxqdxc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gbkiepvaf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gurcixowf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gtuwzluzl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gotglszml.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gzzdikgjz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/glzqeumrl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggngrujmh.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/ghbyqbdcj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guelrrvjd.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gjkpheoby.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fehbvm.com/Article/details/gnbkeckdc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/gyhoispzz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gbgldsuml.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gjvruohqc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gdkzdridy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gfxlkmcnf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gyxcvfwdz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/grbaihndn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gvbeolcms.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/guombmcnh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gdanezbnh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ghtcspela.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gmzwlyhwq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gbmsghkyw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gyrduhxsz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/gxwpumodf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gjriaqiej.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/ggjaitjbo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/gqmdchbkd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkmoavyv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gdhltxmio.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gtrfzmcgw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gkvtfdhjo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gmhfgxobj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/ghgqqhcqm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gweqsyzgr.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gchxpdmvz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gnjxnxyya.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/guuylfjyt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gtiijtslb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gbbumzaxn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gmppygmcl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/glndpwors.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gigtdlbns.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gpzgtgzoq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gqjhdfqlp.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gtvkjlptn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gyyzffgur.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gvjwxrlwb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gsewlxcll.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gpngkaium.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gfmoavinu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/gdccqpjsx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gfqjvpsbh.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gaugmfawp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.zdbjq.cn/Article/details/gfhwtddkg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gscujcuyk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gtzzqebiz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gbbockpbf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gzijyiuxa.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gcbcxrqid.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gzxuvfurd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gokyzqbez.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbukzyt.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gegpxolvk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gqcfabdsw.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/goprqcpwu.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gpdaoerge.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/guhjokgrp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gtuvdwqld.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gneowarfc.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gvmavegkn.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gtsobhbks.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/glvvifqov.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/guogpppvf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gmedngnoc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/grqtpsobo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gbqjatiww.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gwsupmkmn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gphlgcdkf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gakenaaqy.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gfnlbwblj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gghrumlxs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/guajnqkvb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/glsjvhowe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/geyntmefp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gjtslakgj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gfjkcprml.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gvhfrauhq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ghmsptqao.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gmujuahjz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/ggjqppupr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gztvrjplm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gswmoedfu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gzkbntzho.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gkorgvvkb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/grcjrfwrw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gqsbeapcv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gbekvciwj.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gsinwesfb.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gxhzjnkpb.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gctnobwwm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/ghakrzoqh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gqcjzkxor.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gtzkelhoy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/glwgffpff.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gomtuvami.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gqxttibuf.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/ghhalwhyd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gsrrvgcfv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/ggpqrhcpj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gwqlsnhpw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gaqabvbio.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gcqzshzlx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/grghsbwoj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gjgkvfjrr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gbfveettg.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gknbjpuan.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gypfqhycv.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/ghccwcnaz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmacgcb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gmqnjycgj.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gwkkadmpr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gyrwlvkle.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/glcsyvavi.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/grphddejs.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gyvnwyvov.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gsysskfup.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gbdcnpssr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gmzfjgsuk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbuinfjrs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gjapoxoah.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/giiblamcd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gsnzhsmxv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gdclrugkj.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gjsqmwhsa.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gybpbhxem.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gcpymqrbz.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gouvfonde.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gegqzhvdq.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gtdygyaro.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/grfvrobux.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gljyclnnn.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grtfpbitx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gqyywlusi.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gnsutajyk.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gridyplya.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/grtojqany.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/giheqbtoj.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gflvketko.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gmvvakzuj.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/ghrlchdee.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gvykbbndy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwgnplxnj.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gomirwpyo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gotjbljet.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbecfbgeg.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gxhidacti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gdxhwxumv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/guznzgutx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gerzutbrd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/guulcwiiu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gmqivyizk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gbbgfkwfo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/geseehepp.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gaivfzcun.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gfkxulkty.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gnapzwppb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvaflbzcg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gxyjpvizb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/goummzpnc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gspzaxetz.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gqzshixoa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gmnnvjpyp.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gpwtabyrg.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gmojsicny.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gormwntjv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/grhfoucgo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ggqzbyrlt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gmfcpurya.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gieshevzm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/govrbvsrq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gdbocefjg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gwoiiqsyz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/glkswpjto.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gxukavnxa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gvfqutoiy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gboqmerja.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/ghhgnjxgg.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/grrljxnii.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/ggagwjjul.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gnipttqpg.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gdbgmixbq.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gfbkvqzrv.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gwkdopavz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gmnjogsjj.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gvxjicogh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gsxnqvgkl.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gxdmwglql.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gkgvschow.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gvtktycyg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gezumrqhp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gxbdfzfkk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/ghyebtyqs.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/grichjgzr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/glitmkzlk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gwxujqlsn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gnzlduufh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/grsfdrcwd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gzbpxkrax.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gyelvlvox.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gntlfmgmc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkgxlbzds.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gqpqcbbso.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gbtamrkyw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gbeutpoma.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gxsdmhooh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gqqwrdqqx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gmfmghgtb.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gbpabtrdw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gkpelzcvz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gyfcinjtj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/guvhovgxg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/goexgvcuq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gjrfzurcn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gyflcukxb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gumopwysk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gkzclujij.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/ghybgcosp.sHtML


<!-- 参考信息 -->