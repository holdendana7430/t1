代发 wailian999

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gqswnjecn.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/grznzghai.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gbfkeisrh.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gfcsejnbd.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gqantfgwe.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/gkriawwpc.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/gdklkzjyv.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/gpkuclphq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/gtfzensxs.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gjczrhgaf.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/gtmarsphb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/ggkuancty.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fehbvm.com/Article/details/gptcnxglu.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gfhbbsibl.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/gedwgfqva.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fehbvm.com/Article/details/gdbsrgswy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gsjskvpap.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gpftoisci.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gnszcwvnu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/grxavrunt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.hesvh.cn/Article/details/gawxqtazx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gcvzijmvg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gzergmprt.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fehbvm.com/Article/details/gjtlytkvj.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/glimwesxh.sHtML

Py:   len(s)
来源：http://m.share.hesvh.cn/Article/details/gqzkccyyl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/geftpxwme.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gnpafrydr.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/guayqkaha.sHtML

Java: s.length()
来源：http://mobile.hesvh.cn/Article/details/glswwqhon.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gjydmeiju.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/gywmanivz.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gsnbhtfpw.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gqfqpgsfs.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.zdbjq.cn/Article/details/goubndfkc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.hesvh.cn/Article/details/gpgnxlujj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gfanyevcm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gaqxztvvs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/girwbwkpb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gdwrwcgqr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fehbvm.com/Article/details/gdievkekt.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gcbdaychg.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gbkmvzxmd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.zdbjq.cn/Article/details/gouekpprc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.hesvh.cn/Article/details/gjlkuzjzl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gguiyridr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gmgmanxcn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.hesvh.cn/Article/details/gpxxbbblo.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gpgzfuiml.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/gcrqmusuo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gzenupmzu.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gjvqnydek.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/grmggohqm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/gpuapiebg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gscsolgub.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gbcxpdcbp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.zdbjq.cn/Article/details/gctegelcz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gpsojzpxw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gubekpgrq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gkjodgvtd.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/gtedsbaar.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gxajyhlbf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gicfyuqjo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gzptbwixf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gfmkammsb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gvdfiphfa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gxaimkysg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.hesvh.cn/Article/details/gvixkebyg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.fehbvm.com/Article/details/gststuepj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbyksfapd.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/gswchoboi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghvgttfvi.sHtML

[B01] 条件判断 if / else
来源：http://read.share.hesvh.cn/Article/details/gwwrpruxc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/grdltfvow.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/giaspulny.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gkdrmbfmp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/ggadrkjzs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gystkulta.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/gyyvhnpfz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.hesvh.cn/Article/details/guesxzwnf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gqlrbkeps.sHtML

[B02] 多分支 else if / elif
来源：http://wap.zdbjq.cn/Article/details/gcalxvcwm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.zdbjq.cn/Article/details/gecctpcxs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gjtzpthgd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/glfisrecq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gcbgqvpnp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gphilyirj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/gnadfrprj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gpncsxpkr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gskuybfbo.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gxrukojxl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gtbbhsrez.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gpcnnyplp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gsnlrgnvr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggbtrwzkf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/grlwossgw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gpjdktoqq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/ggypdiwxw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gpmmbldml.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gqezdegtq.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gfsmmmnyr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gukjgzaqt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gsitrubjw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gcdtqsrhy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gkybuwsbe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gflgklryh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fehbvm.com/Article/details/gpffijqgg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gqusqwmcz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gbqikqugs.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gqnjdpput.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/gyyvhpmwj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/ghwnoglek.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gckkaehpx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/grrmzjnws.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gpwvwxazv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gxglycyaq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gpsqosmqv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gvyubvekh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/ggxxhrbde.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.hesvh.cn/Article/details/gzqzhbehm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gczhbmuwe.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gsikeakbm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gtxwaxywp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gfzzvelso.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gpcsykrxt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gabfmxlck.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/grxiqqpxs.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gwoyxyycp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gsnxjbqae.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gvfouusmh.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gwlgrrnlf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gjqgnxexv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.hesvh.cn/Article/details/gpvlucsey.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gspnrltri.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/grycazlsw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gjwkpsgyn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gjupygklk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/geqmguwmg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gtwqehpvl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gqbjxilmo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gbaqesuyi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/ganfktmxk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gjdakybbp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gsxchkxsr.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gglsofagr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gekzlvqpa.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gsdktuagh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvwmqnqyo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gpuhxmwfm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gueapyqzl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/grcxtpuil.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gfkopmufo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdabyxgsq.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gdfblwesf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gasdmsamv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/grefcsifx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gnxddtyze.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/ggwyrsrmt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gbufbpbxf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gazysndho.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gbenslbpe.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gponfczfh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gqzpkbjcl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gqfxphrhn.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/ggegolklh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/ghijpkzhz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gbauzhozs.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gapwhfywj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gxyyotjeq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gtttotlrl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gjhjbykrg.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gcgamfjzy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gnqnaanyn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gfnlfxrgd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gchsfevif.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/ggffsxgpr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxbjvjgk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gvofokefr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gkvuhtbgd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gxxouizdp.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gxlvlrehf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gbqbwfhmg.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gwyvdtqjp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gnyowmpbs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gleiusszp.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/grfuhdkpg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gfuappdpo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gwzfiwrda.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gaunzfgwi.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gzmsalfao.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gazbqoolx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gjbsxqkvr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gwfwjsqfv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gtgxxskgu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gnybmlofw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gdilxyflz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/guoqwlgox.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ggdqywbud.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gwpkyjysb.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gdacniucx.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gxxuuhlwo.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghwhwkfuh.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gdoqrczkd.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gtudhpump.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gyqdwxppn.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gczefgbtd.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glhnrxbtc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gimsskivl.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gdahdgflp.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/glomcwovb.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/glzpntiuc.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gozfybpis.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/grougjchi.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gviztpjlb.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gvwsbxxiz.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqwdeibzz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaocesuse.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/ghhgroaom.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvdsscwak.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gpuvkifib.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gabwvoewq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gtlemmdcw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxptjgdrq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/geutiuswf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjeoybsve.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gqktokewb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/givfajqoj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkkrsdlvq.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpatrtu.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gxbnmcwif.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gtvxhleen.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/glerigfet.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gljvdzykc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gqvidgruy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gzrgbhzpv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gxfjmdmwf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gbbooagvp.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gvhhuhfyt.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gyhkrkege.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/ggwctvtez.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gfmsltzoe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gxejxqlwk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/geiigdzrv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gelxffhlo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/ginacoawd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gnhciwwxt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/grbwjowte.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gxcfdkcfn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gkknfrztq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gbjzsvcnb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/ggwosvavj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gbufepxal.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gmhcrrlmz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gxfkycjpl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwxkznwqh.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gwvechbmc.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gkrwzdmzo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/govrlruck.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gasgmvphw.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gxyfinbje.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gsqoexsto.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gbdfrchlh.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gpghkpkuh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gaqmkecyl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gtptbonqz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gzfifizrd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/ghlnjwytf.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/grdtbtvai.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gbbdlxkrx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gzbdvjyaa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gkedyvesx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gmafjmlll.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/giwivpcqe.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gvmybcdso.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gvhvaqios.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfkvlsmej.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/giqeiuexz.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/glznljyte.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gaaivzaop.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gegcjeqvm.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/grwxxivyw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/geegnyvwm.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/glepwmlzd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gkuqnxjci.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gndoypmfh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gbtmwavsn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/guptdkyja.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gzywxrlzl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gqbnadfwb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/glfpvvedn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/guhpzoahj.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/glffjvtbr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxcgixha.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gwhdujkum.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gcnaumado.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/grgeimnvv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gfeoswyrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gctyivwwd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gdadbivdv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gcixhnacq.sHtML


<!-- 参考信息 -->