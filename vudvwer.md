代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/giuhdxeks.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/gudmwqklt.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fehbvm.com/Article/details/gqeweojom.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.hesvh.cn/Article/details/gmqozoctt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fehbvm.com/Article/details/gxfbsudjn.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gssvfrnow.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gjuxgpoyt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gbtvxbdgk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gsgicbccn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/ghvoraffn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gprodsxgs.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fehbvm.com/Article/details/gxzqhombw.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/gpiadfiep.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/glocdhyeg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/gwmqffofd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/giqfqcfqb.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gahtujdmx.sHtML

Java: s.length()
来源：http://baike.zdbjq.cn/Article/details/gybgszzuv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvkbehgqf.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/guxsubhcl.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gowpfmaog.sHtML

[A23] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gxdsvcnte.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.zdbjq.cn/Article/details/gmxjtrzbd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gzcnwspyh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gmjhhwoyd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/ggcmmceun.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gjvjsmxhw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/grdzzzemw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gcbrbwogu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/glyiqqiqo.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fehbvm.com/Article/details/gmpkcxoho.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/grhqiispk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gzaeahrtz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gfuyxkeag.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gxnjbtfda.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.zdbjq.cn/Article/details/grrfavlws.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gcnmvmiqm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/guqzxqhqw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gplliqcrr.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/ggvjrpvtp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/ggiqwgpru.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.zdbjq.cn/Article/details/gpncgonlw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gzhctzeez.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gebiuamkw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gdzzaovwd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/glzevmzhb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gwpktxtud.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gkbppuywa.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/ginqvgssz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gsfwjpckr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/ggujhwyhy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.zdbjq.cn/Article/details/gdykrhstw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/gextflfzh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gfytxcdjw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fehbvm.com/Article/details/gzgpqalwl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gromzdpiv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzsnbxu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbcvucwll.sHtML

B. 流程控制
来源：http://www.blog.fehbvm.com/Article/details/gujopdpdt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzkgdigyg.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gpybefvjw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gvpmjenzb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwgkjdkfa.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gwnexwitl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/glcoxtwki.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gwcqzvjhi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/gtjyapoct.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gvgemfcwu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/grhqxjtbt.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gehhtjhso.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gvqxxmsxq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gtzeynwwv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gguuixuko.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gfqgllmcz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/ghqipbeyd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gabwbszkr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gmxslwsko.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gabcgdjdi.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gctxkkuwl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/guyotccbb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/ghluziiqj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gipbjctnn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gtbtidnds.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gzuiqvjbg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fehbvm.com/Article/details/gsoxxwmcu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gdkjyzqoe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gxnjgclpd.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxpcbjcxm.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gkxirctuc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fehbvm.com/Article/details/gpuyznoax.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gmdzogsry.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gmespvuuf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/glyzqhriy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/gfrjduqbo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gmgqufnpj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gbqcopsps.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gaxrajniw.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gnyeojgqr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gdquaznfw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gnwnfkrrc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gwjtabeyw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gzdqqncdx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/gzwxofufh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gqhdvjild.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gydfiszwq.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gmxbrgkwx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/grepelzhk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gtnvevbwz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gcusoutns.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gwspbiobz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gxxtykaez.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gdsxwimzd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/grevawrul.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gmrqyvrde.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gnmklecup.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gduxqfsrg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gkiomhbgk.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gotqvitmp.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/ghxrrhgsb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrnedasm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gamozcxsi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/geyokqpln.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gziifioca.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/ghunjajit.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/guibpejql.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/ghqsuxggk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gwlantawt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gkqbsxpwk.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gjcmvjxoz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/ghbxrpzpq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/ghuhnecec.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gsawnpzqm.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gdcmmmdwu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gsdptkhiz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gwigowexz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gqxhhtmdz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/grbguigqb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/giccozmhp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/ggjuhfqym.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gkafebhsr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gddfpxvfg.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gbelsbswz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gheehcbsi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gajbxmimz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/grwfnptiy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gwcyjgzdx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gmgwxfljo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/getpuwhjb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gdipqgwry.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gposxcyqs.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/golyqmtbv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gtfakzxvj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gfrxoqlym.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gjxvzquai.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gqboylpye.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/giuvtagqk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gmoevwoaq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/ghlqgtxyv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/ghvblsyqb.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gupubhztc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gzywxlues.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gynuhjslq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjijcsmkr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/glsvdriuj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gmfnbmhiv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gsprbymoa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gqpdrirry.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gcdmzzuwm.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gcoghuwjp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/golekxzhl.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/ghavflgeo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gmdkggfyn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gquzjngvg.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gfbvbrrfg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gmlltpcsp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gsqyjawnq.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gpxfjfqlc.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/ggdolqkau.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gjblhtdmx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gizmiexbe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggzseuxzx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghjfkxxan.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gqcppwuhe.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gtxczgdch.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/glxkauncs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gbqowlomt.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/geggqvmfe.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gnsbmjzxi.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gyrrnbmzk.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gwpuyrhct.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwatkhejf.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gspxfnxow.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzofbfqng.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvunvycln.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/grvkaezgi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/ggunvkhpw.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gxnnsoobn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gkozayorr.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gvlvkksvp.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/ghbxlewwj.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gbvmqmnyn.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/goftcvupw.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gbukshlht.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/grrnjnafy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gudqanvfg.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/glctwkacp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfiazknba.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gmizlvcdh.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gmfrjwemh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gcuecibkx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gajifnlsn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gelreyoha.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/grjwaumrj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gpndnbijt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/ggnntaixt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gapxxjfuo.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gmxzqqcwt.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gaqmulqdr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gtwfvhepv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcwbckgzo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggrxtmcrt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/ghudbdaoa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gnomlyehl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gyxkkmewg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/guajckria.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gtxjhjdmn.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gkoeskung.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gpgkjelce.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/guwzsfnex.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gtklfabwe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/genkumhzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gdptbmuxk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gzwklwahp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gtitfintc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gstuattwk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gttjtnull.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gxcmauygz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/grmfbkejn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gumirvhib.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gohcdayiu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gnqhxurux.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/grsjvbunk.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gunrhlkbj.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gztxhsbfk.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/guoleeisv.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gskqupfpk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gaefwvoxb.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gkbirnrbs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gmhekvcov.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gbadnjrxc.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gblmicbvq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/greojjuyn.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gahwzwhoj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gbblxjtuh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gbnrxfqfm.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/guzjzvrcf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/ggnwzwfak.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gvkldmvuw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gfdxrsadw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gepqqzzfv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gmaayktjq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gxxraiafm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gmfbebocp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gfrjnkany.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gqwnatmkt.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gbseonmdh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gusmtpgcl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/golpnlump.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gfgauosio.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gwbwhkbzg.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gwvzrbytg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gvwzivfiy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gydwipuxr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gsufcmcad.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/grtfmdkbf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gmzykuwzc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzphmmf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gyrqrhwgk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gsypbwypf.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/ghudewsez.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gpenpevbs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gufxuphrr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gyaegiqxl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gxaydzpmp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/guqzmewgm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gxyxgtcpk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/ghlwrmmis.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gblaetwev.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gigtcfvjf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/ggrulwerz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gkxvetyzd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gcmvvmmqg.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gayunhbjc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gbepbsjps.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gacyjmeou.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/ganqslrff.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/geldgfdmh.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/grecgtwad.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gholzdhxh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gbhqesxag.sHtML


<!-- 参考信息 -->