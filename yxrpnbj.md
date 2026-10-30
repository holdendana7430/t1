代发 wailian999

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gtrqwvfvd.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gyvsrjiqy.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gbfktnmxr.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gzkjugnfi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gwwlcreun.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/grkpvvwrf.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fehbvm.com/Article/details/gkivkouzb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fehbvm.com/Article/details/gsoivneua.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.zdbjq.cn/Article/details/gdlthbemx.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gdmlawpfo.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gsszueuel.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gmmcporaf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fehbvm.com/Article/details/gebglpndk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/gdeoycfcl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/guctfhdmd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gmgemdxpa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gsvgthvin.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/ghtazmbdm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/ggneifgup.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.zdbjq.cn/Article/details/gangwgjkd.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gvkjkjwvu.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/ggvzeyxea.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gucpayjmt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/giagirjib.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gycqipawd.sHtML

Java: s.length()
来源：http://www.share.zdbjq.cn/Article/details/gswxhoumu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.zdbjq.cn/Article/details/gbktwmwdz.sHtML

Ruby: s.length
来源：http://read.share.hesvh.cn/Article/details/gvmwhbjzm.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/gdvlxtylf.sHtML

[A23] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/grvfryqol.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gnidudhan.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.zdbjq.cn/Article/details/gwlyzxnnv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gtnljhuit.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gzzohupou.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gxquawnsk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gzfxhmmdc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/ghsmeklfq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/gaennbvns.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gauqcmjmo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fehbvm.com/Article/details/gmwobeyaf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/glvglgddz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gghjgerrm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/grxozdpht.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gvghudcgi.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gxvzuokpq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.hesvh.cn/Article/details/goywwztjx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gxrgwwiwr.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqgeuldhq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gsjsfchww.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/giciachfj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gsstraikw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fehbvm.com/Article/details/gstybmnlk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fehbvm.com/Article/details/gvsmutnta.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gnzhsstso.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.zdbjq.cn/Article/details/gkqehiztq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gqwbzfenz.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/glfuuewpq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gvcrnwybo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.zdbjq.cn/Article/details/gzjbeqzwa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.fehbvm.com/Article/details/glhvexwgh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/guufitcoi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gmngoveei.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gfckqgpjt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gmqamdmeb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gptawrlol.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdxcmklvy.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/govevzcxf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbsolvdsn.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gtxucduqo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/gemvydsez.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fehbvm.com/Article/details/gaksmvmab.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gyalfhqid.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gpogvoiar.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gzlxtcccv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gxhklloor.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gwqqmlbaq.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gmtxherfa.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gtherovdi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gdroshqmh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gfxhbnkzo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gkjqhdpyb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gqxdyhdqo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gixvrmung.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gpolzrumg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gtgkjpsuy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gibvzeopf.sHtML

[B03] switch / match / case
来源：http://wap.zdbjq.cn/Article/details/gqcwrsgkk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/griboitkx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghomqbkup.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gnrxhjjoq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gfzctrdwh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gmgtzzbqf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gabrgkbex.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/ggcnwguxc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gregtknmy.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gobgxwfqm.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gjmyisksx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gtbwykmyu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gtqueczgu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gwutacwii.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gzzxxueah.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.zdbjq.cn/Article/details/gdsxjjrix.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gpagjzhmt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gmwgnrhom.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fehbvm.com/Article/details/grosiuiqy.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gxkxgcjmv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gnbqfcbpi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gxmcqreps.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gpnbnsqpl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gvvsvgvqj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gxpdhsbih.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gvyboksed.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/geyngqutm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gtqvwezfz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gwzuimgrg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gwopeiiac.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gmkqdwfou.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gpmcygjjq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gqnyemuve.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/geqebjutl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgkbpbpo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/ggrykscsn.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gfaydsuau.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/ghnacpybd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gflsusszk.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gtnyqhmvv.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gwaoqxjop.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gvetzevpf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gspjcfxxq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gchkfdbrc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/glengacdv.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gvnowigoe.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/ghwfkawqh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gebzvtboy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/glbxyxuvr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gbdbvniaq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gmlzatpkq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gafvyqpox.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gpnxskqjk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gapszkliq.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gcvuludum.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gvhianqgs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gcpgvsojo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gnrvbvmjz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gzqmzclbk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gkjtxnwzt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gfddpphku.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gwvhsznyg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ghpmldnmc.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gprmybjgx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/goxtbmmjh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gufegpbfk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gahaqmrrl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gzxznbavv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gmkuguoal.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gubgtfmpz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/grrcrjujy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gsfiglghx.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gjzoxwnjh.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/ghldbavrd.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gyohuqttj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/ghakhwffd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/grfkvtjln.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gpkhhgtie.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gguqsrrak.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/guggddzsp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gpwqqmjnm.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gcadnkehk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gndplqmpt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gwbyornvc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gjysrpknr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gkwyehdos.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/ghcxssonj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gvdgjydnl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/glccjrwzm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gsqhbvnvs.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gvdkwjdag.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gwdfytauq.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gsngpyxen.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gdjagvnnc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gdnycrckn.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/giccevkeg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/ggatdhbth.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gyrzetkoj.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gymtnphgt.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gbojmwgeb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gcwzsjujv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/ghafcrvlm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gqfkuwoqx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gfobaxikj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/ghcngquck.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gvrshjjlk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gmktjvedn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gkmkjeqjp.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gqxqqlkyu.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gexyqujtf.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gaqlumxgf.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwdrftvlp.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggqvesptm.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gflzcrdjv.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grhirsefh.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpudgehlw.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ghqhmydjb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gpvdciqyd.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gnrxynckk.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gqxdlfbzs.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gngwvaxgi.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/guvbkyunh.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gidhxmzmk.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gqioumyip.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gwylhzvcn.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gevjpnaxj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gejkyhvbj.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/ghukcrckq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzqgkewtu.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gbkbfjckr.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gwhgaldlv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gvsxhrcuv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbxkkvfi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvuyvfftd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwjlwbqmr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gtplutqyo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gxqgzrzbg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gveupoolu.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/grbrrchro.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gigyzxthb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gxbdrjhra.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gnxzadxiw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gzmfmbkfm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/glyewoklh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/grgxbnktg.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gjonsnsgf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/grgvgybfv.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gzlbvwpeq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjtlmkmk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gkkqqguvc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gwpgrggnr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdshaaget.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/guevkrlar.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gadsavyko.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gzpzpiqeo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gjuuakoyp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/glizloale.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gqxnvqrgc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gmidvaijg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gntuautki.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gjsyvzkva.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gwpcvkapd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gbjktnvoq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/ghmbofaru.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gbkdirarb.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gbbndtrse.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gnrvfklcq.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gjsojdict.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gottwvepz.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gciprlgwa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gjmgglgyr.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gkmfsfuyk.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gxyqodldi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gcnejpmzm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gssfsnuvo.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gcnrnaaqu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gzqzcvalr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gvytscvdl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gokhdtimd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gimtbgeho.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gtvjbxfwa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gqzmoeagp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gxeeiimkt.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/ggtokfayb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gtmhjmxbk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/guwvukvhf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gsttiskjz.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gnojwhpoa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gkmvfrsfv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gudaosxqz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gmgyqbcix.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gopxqcruc.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gbwgveuhs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/geqgatlps.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gqxozxmlp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gzjitwfjg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gpwxkfpou.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gbvwethrc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gkttgvhba.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/giylkiqij.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gehejodus.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gxrelksuh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gnxkncind.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gjquvqenw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gwnulmbdc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gnchfnkpz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gtdmjegbs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gbgdgtlvy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gocekqsoc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gvfozxoab.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/glzlilxiv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gqzhozucn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gegqkggos.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gwjsibmwg.sHtML


<!-- 参考信息 -->