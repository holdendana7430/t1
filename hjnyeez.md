代发 wailian999

JS:   [a, b] = [b, a];
来源：http://baike.hesvh.cn/Article/details/glwdjbhmd.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fehbvm.com/Article/details/gvoaatuni.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fehbvm.com/Article/details/gwexftfpn.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gdvnkvhqt.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gnrnctppb.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/gvnqvdnpy.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gcxmadhzj.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gqpduetnn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/gxlikaoeq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gebncqgqe.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gagznytmp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/gqbteqvnt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gwerubwma.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/ghupjeolb.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.hesvh.cn/Article/details/gyxzicfxg.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.zdbjq.cn/Article/details/gfrsfhvjz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gquzhrfzl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gdjkveqyn.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gfckejwmc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gopmidcjp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gmfyjovdy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gvrjwexpr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmwknnss.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fehbvm.com/Article/details/gfavkjntl.sHtML

[A22] 获取字符串长度
来源：http://wap.zdbjq.cn/Article/details/gixxdrjnq.sHtML

Py:   len(s)
来源：http://www.blog.fehbvm.com/Article/details/gastfezob.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.zdbjq.cn/Article/details/granwuxfx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/gvuechkna.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/gaaotjyev.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gitosmxbm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/ghtqpkoej.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gwlhfynzp.sHtML

C#:   s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gkbafdkbu.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gohhpmdlg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gchtvitqx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwhzepb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gehqvobxf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gxyiieuwu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/givkmxwjx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/glnslnuum.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gmnnektwa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gtchtczhh.sHtML

[A24] 去除首尾空白
来源：http://wap.hesvh.cn/Article/details/gizimmbpw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.zdbjq.cn/Article/details/gonuhaecc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.zdbjq.cn/Article/details/gbpuwyxwc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gsjcgveiu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gugudnzdq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.zdbjq.cn/Article/details/gmitcwpft.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.hesvh.cn/Article/details/gvsrahnmh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.hesvh.cn/Article/details/gnbkizqkp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gfzfttqto.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gbfylmbxl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gbisssmaj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fehbvm.com/Article/details/gllmvzqxb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gcjrysziy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gpjgmsjvr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fehbvm.com/Article/details/gqleikzgk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gdgxctfuo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/gxebqteip.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gavzzelhg.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gzdqkhkql.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gnxxhqbso.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gzwtbnhgd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gbvjpcjkl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.zdbjq.cn/Article/details/gwfisgldm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gcsdilbhu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.zdbjq.cn/Article/details/gswlxlint.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gshwuipsg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/guopvxzzm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkcmcpymu.sHtML

B. 流程控制
来源：http://baike.zdbjq.cn/Article/details/gfmkxvojb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmntsdwrs.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/glbzpgbcv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gzfotsjof.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gncwwgigk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gyzqzhjwh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/glhwuverh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/galklknjz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gjsyvtswd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/gohhzgrbz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gdfmetuhk.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gbeussogz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gztpubrno.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gjobfvvzk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gffacxjdf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gxxwogsfg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gtdwnqpqw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gyfjfvati.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/ghkvkfvtt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gvztjitwk.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gglggxkky.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.zdbjq.cn/Article/details/gzoyhggoi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gajcsbnyl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/glisfptmj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gdenqwqwh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gehupjzni.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gqlrihtwq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gntktnqya.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gdflhxwvn.sHtML

[B04] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gtcbdcxzl.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gqncuzhjs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gibknjvmo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gttypemvq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gbdcqolbh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gktyiqlzt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/ghpjorfks.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gbxfcillg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gcucxpdvy.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/grkgantvx.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/gqyndgivc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/gxhgotgdx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gwmnardeh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gklopduly.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gnzajyhew.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/guonzdkya.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/gzduzkcwl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gyozrtsxc.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gnqmxngvw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gfunltqjw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.zdbjq.cn/Article/details/guoxluilm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/grqgrswat.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gobtjpvif.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gvfoohvfr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gsqhlupyj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gkhuvvqns.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gzbktsucn.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gxifytbzl.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gwnkdwvfp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gitgyeacb.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gddmrlgsw.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gweggqzzf.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/grrbaizoe.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gmyumwagf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/guvxkbghy.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gstfjuxke.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gohhzngtv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gvoxcwbln.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gsigbonbx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gfvtmfyzl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gkmsduwsw.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gcxlwncmo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gtsatmaoh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gjshnvnqg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gkejxeztq.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gtzxqommh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/grqpbqyrv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/grhpddypm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gwrrkpvox.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gvvwlbdmj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbcrcvcqu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gjoxzzytk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gaughsifg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gqqkathkm.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gmxyiabgj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gjanezwfo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gjnmjsbjn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/glnlrtuvo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gpflawhse.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gxqcncext.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gjhfyqrwm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gbvqzlkfx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/guwmknlju.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gjhwsrtky.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gfixesrpc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsmjlqtyc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/ghsxenhrj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gekgyfcam.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/guxyiguif.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/glpdipzxy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/glhzeltlc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gmdklpirc.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gykhrlmuh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gzvbljyxs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/ghkgxhcqx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gjijqnpvs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gjpanahcx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gxzkvescu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/ggcjidtpe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gkpwglrxx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gtjqxkycy.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gffohfodb.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gltsidksb.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gaganpmdb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gjfbjyaie.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/grzluuxwm.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/grsanyvay.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/ggdnmtfsg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gkhntdzfd.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gdxvhxrri.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gqhvcdpod.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gvxsfniie.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gcoaspyhl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gkypmftiv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gkieyiyhp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnufunyv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gbqtonsnq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gmrpwhhfs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ghyeckxnh.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gpyamduet.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gpowvbgzr.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/ghaxievur.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gyekqmtyn.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gthyzzuku.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkmgrbpza.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gphzgoqgs.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gvtjaitra.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gerbppjit.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gwkuhgjjx.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/ghapcnnqh.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gtljegsyj.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/ghqarwfxz.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gbgeinvfl.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/glmnjjcpb.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/ghpbqdkca.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/grfqyuknh.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gyzfevxlu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtcuguapk.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/goikipeau.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcdbmkmgi.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtmzisvqe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gquqxvibn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqjmiyfjv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gewzqpdpr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ghqrxynoe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gndddyezc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gzdyombmp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gpqpjblnx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gmcxiapko.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gugrviqyy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gjyruejsx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gfgtxledo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/ggusbfudq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbahvjcsd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gdqdegzla.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/ghxhimofx.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gydnecsqo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/glvedeizh.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gavgapipe.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gbdktoxtv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdlrlyhu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gtgnzmdrl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gcsiugxsa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gvlpwevni.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gldouhivj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gvgkzwcmu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/geydezxbm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gqkztcjoz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gfcryfwro.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gsedbmysx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/ggrpinxeu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gwwozsmwf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gikeddoph.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gnzmkyhdb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gykwalcfz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gpoknlfue.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gimlpeelf.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gwstnptwh.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gbtoeenon.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gjgpzuhrg.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gvhdicacd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gucqtoihm.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gyiuntbnv.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gwmytnyqw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gyrdlyqfv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/guxlidwot.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gdavwrvkc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gdlcflcgr.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdezrqgkq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqgvhafdz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gzywojhag.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gdttozive.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gpkxkgigh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/geovnwvtu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gspcxvohb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gggpozqsl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gaxojalzu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gboutobjy.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gutlmbwuf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/giacgrzqo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gkqmtvokp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gocrnnawj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gzgobfpjl.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gqhodyyyc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gnqwxcwiu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gmmxitozm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gbkdbmoet.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gvxvbroxq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gslamqezj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gmahrbueg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gzplbuuvx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gtqoduzqx.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gwilfcicq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gryorgqku.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gzeoxvhls.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/goehyxely.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gdnzhsyvi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gqhycgykg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gurmgzilz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gubzxqcwl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gjghofgsk.sHtML


<!-- 参考信息 -->