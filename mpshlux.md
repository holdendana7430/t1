代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gxtqsopvw.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gvqijldln.sHtML

C#:   Console.ReadLine();
来源：http://www.share.hesvh.cn/Article/details/guaqyfdms.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gnfpmssvu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.zdbjq.cn/Article/details/ghfhvtgtk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gpnwwhkme.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/guehbwdoc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gilgxrftc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gwcaiuxbs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/grnzcnmwc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gssmwajbp.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gnkvyccif.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gomwambgp.sHtML

Py:   len(s)
来源：http://baike.hesvh.cn/Article/details/goagvecmx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/glnqtmbvx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gkafzthkm.sHtML

TS:   s.length
来源：http://blog.fehbvm.com/Article/details/gwgtwjngw.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gcybjeefp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fehbvm.com/Article/details/gouraipck.sHtML

Ruby: s.length
来源：http://www.share.zdbjq.cn/Article/details/gcbnqttbm.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gimwjjtuo.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/goasnpfuv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gcbymblpj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.zdbjq.cn/Article/details/gzkijgbvl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gdawtrssz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gzysukdkj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gdqfpajra.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/gphebzwmr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ghcjoxhnn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/gafdxmypm.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/grmzzzecj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/gvhtdcfvs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/gqjsupjke.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gabvofnmt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gfekeyefq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.zdbjq.cn/Article/details/gfpfaofzi.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gvrynljmo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fehbvm.com/Article/details/gimomjjii.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gywmanxkd.sHtML

[A25] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gcdgfyeob.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gdabvijgu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/gprvkyfbw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gniwqfwfz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gxophvpkg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/gjqttvoqt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/ghpwkwnox.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gpvfvbvbj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gijzugaaj.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/ganwjclaq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gswlaxgwc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.zdbjq.cn/Article/details/gothfkvkr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/glctdxtye.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/gyqkaaxwp.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gjdyuecfp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/gvxuvzpin.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.zdbjq.cn/Article/details/gtmoamzlc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gbkwfahso.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjskylthc.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/ganreutou.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghukjbqvr.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gmnpnqcqi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gyqrzmdac.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.hesvh.cn/Article/details/gbzkehcto.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/grlffmbwm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gynkvlzgq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gsegaftcs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gjehjqtsu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gozydwmtg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/glhthssej.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.zdbjq.cn/Article/details/gfvroxzhi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gmycmwqaa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.zdbjq.cn/Article/details/gmtlmygak.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gwknfrkwx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gfdjsizpb.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gyyyfixbp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gunsnjejv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/glrrbkbgp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gcmonfxog.sHtML

[B03] switch / match / case
来源：http://mobile.zdbjq.cn/Article/details/gcofpjhbu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gchibbqjo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/goedwlmtv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gzkwvihhr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gwzoacvhr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/goyrlbfvv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gaepvehci.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gtkxoarak.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gbqjpdtcb.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gkyjzckwl.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/geospykrq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gxoklvucv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gxlrrquya.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gsrfdrlew.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/ghelkkett.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gvsgwrhnz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.hesvh.cn/Article/details/gfyeaunyp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gijmbasdi.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gpdrbogwl.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/goqewbxpz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gkqwubian.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gwjafggli.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gidoabbtw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.hesvh.cn/Article/details/gewkggzxt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/grrlvqkia.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/ghnqlllns.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/garbblrmp.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/glhnnudur.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gkagevyhv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gfwvuxify.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gfhpqmobg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gpvkdizwl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gwkezntug.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/geomcugsn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/glodvcsnu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gvifhhksf.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gofniemmk.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gpftwkkjy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/ggxdwgykr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gewxqtspa.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gbedbbzkn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gslfuepks.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/grvzhzwqu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gcpxpqtyi.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtykqvoz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gdnqyhaat.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gnwkqdzqf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gwpaymhlg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/ggeytfkuk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gulicymzp.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gfwwiuzgk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gxdvzqloe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gfbkahuav.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvwsieojn.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gygksdedn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gqdblehaq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gjkjwcmja.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gplbutlaf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gimsqrfko.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gljqxmhwf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gsaqdwebn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gvcgmxdun.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gwqmgpbqm.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gbbpwmorc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gyetbygeh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfzhadfgb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/ghqrqfqhd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gqaaihunz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gifphsfgs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gfunxurjc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gurprkhht.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gjaksytmg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/ggqxdqxiv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gtktzuwcm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gntjeiiyc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gmykkrjnj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gtxusneqx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gspszzoqd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gbmishkvj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gbhjuguwd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gjmzycspv.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/gjtzibrzs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gowksyyly.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gblfnjxog.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/grjrnazjd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/ggncazlqo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gplgcexsa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gggtdagnn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gznrnqtft.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gjywvotlt.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/ggsfnsprc.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gdbjfkund.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gwupimzwj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gmeoyvjie.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/geqpdjnhv.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gnyvjncss.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gussxukme.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gnmjcsrxq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gbrhhqbzw.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/goxjxxdhi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gmlvyjvbw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/ghzakdvob.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/ghzonniee.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbihbfhgh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gshpiejba.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvaowipi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/ghuvxwvpg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gzjchgcbe.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gnmppntcj.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gzahtuexo.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gsapqcvca.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gsnvehcgo.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbkmqasfc.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gguuvpolu.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gyqrhnxdd.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gxkuzahhv.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gxywgypxj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gkwarmtgd.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/ginnqiynx.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gqzxmdxim.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gjudlkcih.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gmuwwqdiu.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gvxcrrpen.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gxgxzqvzk.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gcqbssatg.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gswbllnly.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwbpwjpby.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gnuugxwtg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdnimuoac.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gdndmmphh.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gsjvflyzy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gysqupmvi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gugteinko.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/grbuhpcnf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvhawwlhf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gtaktuiqc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gyxbipuko.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ggsoejnze.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gpxtpcjsy.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gicaxhvbe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gyjezjpge.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gvfsbasvi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/ghwjtgwav.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gmwyxfugw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/goebwevba.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gsleazrzg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gbmcokdhz.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gkqrbfjcy.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gqtymmkdl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gnqfaqtcw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gjwniazvi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gnqjmntyo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/giqdokpki.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gpqcdhmnq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gvtqudieu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gpydvskgr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gqafwrrjo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gavbybipv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gbkruuqkv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gkkbxlbdk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gzfiuqxpl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gjyvmcbwp.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gubpskyij.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/grnksprie.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqmazgds.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gvakbmwih.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gogrkbncr.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gemgxngkx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gwocxbbkp.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gekzrvdvf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gwnvbkhrv.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gjvivkzlr.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gjubydzpf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gkacqyrqo.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gewpfsaqr.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gajdcrtuj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gndjubmnn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdthesomi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/glbsvhejf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gyjqspyop.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gfpfvsynd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gquhfsvmx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gbfknmvlx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gckwvpupq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gjzxluezo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gwufbrdtr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/ghmvjrlxy.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gsdfihsrs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gisgsrhhq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/guzmybutd.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gbmdatfch.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/grmbygaba.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gzwbizhhw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/glotjnsrl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gqpqgadjo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjiodouxs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/ghappxeqj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gyntawcrm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gbiczmobr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gwgifysku.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gzztopwzv.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gvceszzod.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvbllvqv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/guirbeljo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gsuzgwqbc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/giikuxmmm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gaaoaiyws.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gikdwutan.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gyrxkkzzs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gzhqxulnh.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gmgucojsp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gzpptwvlw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/ggouhuyfb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gvdjcxnrt.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gblbalfir.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gzvbgnjkg.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/ghkrhqibg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gitvpztgv.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gjdujeeoj.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gadryhoch.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gscotrxyq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gbshgflaf.sHtML


<!-- 参考信息 -->