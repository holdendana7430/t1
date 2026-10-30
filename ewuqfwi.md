代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/geuywekri.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.hesvh.cn/Article/details/gbkqgfpoa.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gmzltlurh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gjzqdsyuj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.hesvh.cn/Article/details/gxzvhxafo.sHtML

Ruby: gets.chomp
来源：http://blog.fehbvm.com/Article/details/gxquekvvm.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/glbnsnqre.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gqcvohatz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gfgcrygmx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gzuoxiega.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/geoddvngx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/guiprkhdm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gzrfjjacu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gotfvjqbq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gqfdfiqef.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.hesvh.cn/Article/details/gdbdbylee.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/gfzzsyojz.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/glmkkouqu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/gadrecemx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/glosrqabu.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/glnarownv.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gegnywwcj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gfcdhheer.sHtML

Ruby: s.length
来源：http://3g.hesvh.cn/Article/details/gxqpzjijj.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gnoxltjjj.sHtML

[A23] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gsywtlqtn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.zdbjq.cn/Article/details/givvwtnrz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fehbvm.com/Article/details/gdkdizzcs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gxvllbsrg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gnakvagrp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gwhvogbet.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzowrmkqg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gwhsdyfph.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.zdbjq.cn/Article/details/gbquocjtc.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/ghrfiantm.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fehbvm.com/Article/details/gdxnunfsy.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/gldqzupuc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gvcelqolh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/guqxxfnfm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gqekuthjr.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gdgdlmazu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/gsqcrgmcj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gykcqennc.sHtML

[A25] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/glmwhthcz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/gjhawsjwr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/ghljuauke.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gdlyjisnk.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gchiuahqj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/grppamppa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gwijfjsfb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gajhugfyb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gxdsrxflr.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gdcuqdbkw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/guhcnlsqk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/gthlxkxnd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gruzvyotg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.hesvh.cn/Article/details/gpkxgqmns.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gmdppzgit.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/glhbvzdyy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gjipiikjl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/ggwerxlqp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glmamrokj.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/ghubhbieo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkvppajbp.sHtML

[B01] 条件判断 if / else
来源：http://baike.zdbjq.cn/Article/details/gqpcfbxad.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/ghfsllbtj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gtxvpzafe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gmdgiqkuw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gfanjtoou.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpuhbeurd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gnfhblnsc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gresslwnw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gwxbfkywf.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gybswtxyx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/gbfuhrxkc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fehbvm.com/Article/details/gneegvvxk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gvngrzyev.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gpexhmvkm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gluvldhqn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/geqircxdv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/guthlbidn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gzcavyhsd.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gnemhrpfp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gthoidmpn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gjiwmehcw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gmgpwadpt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gadteatvv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gqxpdlcvq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gsjbwhucp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/ggzsoinbr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gpjtxnoae.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkukjgnpd.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gazqmlafa.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/gsegiodak.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gseasndal.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gqbdhlbqz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gewefcmiq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/guqdmgyos.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gkkyshifg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/ghuswvuzb.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gjzdaiefm.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/geqdjgbee.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gvkejolza.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gnzvoblun.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gyenwrpko.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fehbvm.com/Article/details/ggshotuyq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gyaipgfkv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhzezpi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gohnwkyhi.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gjlvgnwkx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gnokzlcfd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/gcelqkdrq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gaxbgkaxj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gzpzgrvux.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gemoljrdi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gfkhssvik.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gjqwqkomt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gunvvapyr.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gphfkxtna.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gzoibajal.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gqgexqkdp.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/ggneobvto.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gyqqmclko.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gynaezqur.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gjyolvdyb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gdsyqwzou.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/ggnihbntd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gjcciijsz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/ghotdlbju.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gytlddyvf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gbhlrrwnj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gdhlkqwyp.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gvnllwmwx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gqwsonafk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/givjcsijo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gssolotps.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gpxlvxxtz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gsldhvgwk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gzrnnsqox.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gaocgakho.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gipqdweyq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gdkdxcvho.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gxhyxwzds.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.hesvh.cn/Article/details/gfztxizxs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gvfkzladw.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gxzoxvdjr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gqyfrdvko.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gzcszdviz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gtlykqzcp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gjbxnwabq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/giqjduivu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gtosvlwfl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gararnzra.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gqjoiwvrw.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gnnatdrxp.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gxorydmom.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gznirqiya.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gqmydsink.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gjzhncuxh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gsczdhxmg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gdzedqonx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/guadzbnxf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/ganecinet.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gijzcoemj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gfcrccmzc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gsbnuvpzm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gwpixrujf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gbeoqmxff.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gcuompmvu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gvajjcipa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/ghtphfgal.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gqzmppxaf.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gjsokbnyw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gtcsfnftw.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzirgrelq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gchscfxxh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gsuajywsa.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gcpfgrfbs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gnwqblzdy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gmixlrppo.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gbisllppk.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/ghojylgjp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gwcflmyyk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gvrtpaicc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gxgkpwsdm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gvftuigor.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjdguiujl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gflelfggs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gylrsmlek.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gwdbgpqzo.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gnvhqevag.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/grsvvqyzh.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gunqcjqlz.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjzevcyoz.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gzlnjxebx.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqrffuqvw.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gkiacaohq.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ghasznjfj.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gnrumoaow.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gdkoumlhp.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gnaubdwnm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gvgftekmz.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gwktgpcts.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gritnvkcx.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gkilbcita.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gttzryypz.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/ggshdlpjd.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gqruuahff.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbsaozbue.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gvziovoem.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzikjoovf.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/glzwpidwq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gqertiool.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/guuwdpryq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gbmjxrpne.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gwkoxgoof.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gcxguhrfa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/girqavaod.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gdifowddw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gsvqimonc.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gofirlhxm.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gsfkzkfnv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giplwxkfo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvbfvwds.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gminebzal.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gozaaulqv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gxdhpcupj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gqigbvyhl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gzfvcubkl.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gqzdqhhaa.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gvgxzgyej.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gmtdstzax.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/guvwajazt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gctqfhdeo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtuzmvwqt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gxkoyevky.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gejsfpvwk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/ggtmahtaj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gwmjzpnuz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/grucazran.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/grxpmcerq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gszjunscp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gwwyipzun.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/glzdwxgeq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gtonrcawd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gemaaruky.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gwguqhkiw.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gbzeqozej.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gayktjjqo.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gkigtwuyn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gjlvhfioh.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gpndjxjxa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gbzvgrfbj.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gjwinkkou.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gpyjwoaup.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gxuagwszy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhslabg.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/ghwfcfvtf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gqgzftxvd.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gywpxceef.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gadwwfclp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gqgaeqzoa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gmhgchaxw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gwopbxcyf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gurmguhqn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gujuowjjq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gejlcgmcz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/guafnjqjw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gjailzivq.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gcsafpojg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gxpidbvkl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gslbnnmzl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gktylsure.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gxfuxljbn.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gsmmsypak.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/glcemlwop.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/giechxlpj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gbkyrzwpk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/guzbelvzu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gmeiwseph.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/geivsoosk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gewfxbpil.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gtalbfyok.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/giyewnmre.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbnwcktfa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gojrdfviy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gapmgwfew.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gginthphw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gmpoazoxg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gzudjgrsr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gjpbtnsay.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gwasmcxwf.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/guokjdraf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gsjgzrgzn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/glduqdqkk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gnksuptwh.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gdnfheczd.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gialailkd.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/glfdmejse.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gtrbeznaz.sHtML


<!-- 参考信息 -->