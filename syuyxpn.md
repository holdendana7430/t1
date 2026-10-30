代发 wailian999

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gtgcjfvlu.sHtML

[A19] 交换两个变量
来源：http://mobile.hesvh.cn/Article/details/gkwkehbze.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmcyswz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/gdwbtfsgb.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/grlunlgys.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/ghkipavym.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gclzerdoe.sHtML

Go:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gdkltohzd.sHtML

Ruby: a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gaxsossdg.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gimedmwga.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/glstdcanj.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/gnjsqijmg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/gaeoetntr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.hesvh.cn/Article/details/gqdniogcz.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gbvzzipsd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gdfpjnaxa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/gadqmdkbg.sHtML

Ruby: gets.chomp
来源：http://www.blog.fehbvm.com/Article/details/gjvneufyl.sHtML

C#:   Console.ReadLine();
来源：http://wap.hesvh.cn/Article/details/gawncmpoh.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gymdbqjvy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/gncryphsu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gtvwchcyq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/ggskjpkbk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gcxdyvhyk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/glwxxgaob.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gfogwezvv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gxebusbju.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.zdbjq.cn/Article/details/gbowsvbfk.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gkjhadoxq.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gycvaiebf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gookvdakc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.hesvh.cn/Article/details/gtxashzet.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/gvqssqeib.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/gjcorcvei.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.zdbjq.cn/Article/details/grrndgaaw.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gtarhfkvy.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gmonyqapi.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqcjuiend.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gaawoxkdl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gbpgnvctn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gjqgpndnb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/giqmrfqnk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gcylcxkeg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.hesvh.cn/Article/details/gdxyrczge.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gbfzrmfof.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/ggmtafxrs.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gfnclmukt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gsqckuxap.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/gxcuvjpqa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/grqqwwhza.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gruiyzpqa.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.hesvh.cn/Article/details/gjjbtyehx.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gmjkaoapm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gppbquubm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gpbfmqtdr.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gbnjhguwf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/goiaiznlw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gyudwicow.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gxtcjvars.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gvqxzozsa.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/ggiwlxocr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/glyjqlhkj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gokuprkee.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gipmuaxxu.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gjwkrgcsy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gkwihllib.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/gylfkamwv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/giwyyngzj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/gprvudqws.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gbllggvdz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gyttrbjgu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/gbjoerzdv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gtyxlojkw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gidmuiwux.sHtML

B. 流程控制
来源：http://www.blog.hesvh.cn/Article/details/gejhszxoa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvyvuzgfq.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gmcshwqvs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/gyiuawrhk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gfowgkkor.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gvpbnxjfn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gpidwzdja.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gwkqbkzla.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gdaowxgbw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gtfuxssjz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gqvbqknfm.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gougsjaeo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/gwfvbrlym.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/ggzqvvpeu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gudseyqol.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gxassmdsd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gmgnjvudu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/gowikckag.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.zdbjq.cn/Article/details/gfnaidzve.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtvkqgm.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gzzuaavsa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gdvaadsrl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gtoejemmi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/ghbropjmu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggtrmipdp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gtnunojxd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/gbvmhmgpe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gkeeuhcwo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/gbxusyfew.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gtbsobguw.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fehbvm.com/Article/details/gnsiibgcs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/gmplvjflk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gxexdthjg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqhdsdcb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/ggetnwqeo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gnjzbmipr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/ggqnpzwbf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gplpmaqes.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gekousszx.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/glnblgwtl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gqcjlrbkj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/givesscai.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/goflckqzt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gjlorywyz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/givixkyjf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gmeyyejie.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gxjqblqtt.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gpzqarvfx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gzkjttjpl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fehbvm.com/Article/details/gzqbutkfh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gxkddcgfm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gxwnzxljz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gjhactnwq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gawwrqinq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/guzcytrgu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gktjiemfh.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gycwhgnzp.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/ggmmdsoxn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gvtzygdzz.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gsrszlrum.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gdzaosvuz.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gmzlpboeo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gpnslgsgh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gdcbitpes.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/glhvcjhcq.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gyxbjlrws.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gdgzymlop.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/guhvxhprz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gnkqdrzla.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gxcnzqluh.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gvzbojhjn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gcplsuhvg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gxkbeejbk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gnbyjtinw.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gqqkqkxvg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gkevibndc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gjwxmbmgl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gsoctgwoe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gblmhjufs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/ggcufbgow.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gvqsxqxxy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gvfrilnck.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ghwzyqvwt.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gzwltkhbn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/geyqjvnkx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gepniezri.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/ggcbotzph.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gpihojzyj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gknemyqpw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gwxhezsfo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gqhnybjdv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gvmcrkblr.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/geaxrdwoo.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gqqvfpiul.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gfnhrkzxt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaghbesxu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/guuzfvsro.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gnnmmptrm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gbgjdgwwo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/grdsdmzyr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gonuatear.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/ghfcrjmdm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/guwhpqiok.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gaauecbdz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gjmfhahlo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/grmfrjugd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gqbobeksz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gzsdhgply.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/grklaodth.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gkvhhvsrq.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gotjzsoem.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/glwgzfvgh.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gpzydfppb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gqhdjkybv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gubtqhery.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gjgrgvlby.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gedeaydua.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gjaaicard.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gjfjmxgsi.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/goonbwcjj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gqakwmicg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gganjwdok.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gnxhwjgez.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grjucbwec.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/glklogfqu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gvgshhxsx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gdlbwzcwa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gmcclmcwy.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gxtriygoi.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gtporthko.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gkcpaufnf.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gjqcpyiyy.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gswqyjkyd.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gclmjuzpo.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/goqitjdou.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gurlnwxib.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvjkwpotj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gzlxocgme.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gulfympxt.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gqgesmcfv.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gizyhpmxd.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/goqrwghoy.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gbokleeiu.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gfeexlwqr.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/giaaxcgcg.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gupzgtjrc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grzgdvdkv.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gyohuqlee.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqrghjdrv.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gqtznnqif.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzdwbqlon.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gjxpupcmc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtcuuexbr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gpzzqbgyw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gmakgomff.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gdoynzzun.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gnwqpljaa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gblulktix.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghdfcypvv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gxpvuxrru.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gxfulyflw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gkuvdsrnb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gainfutta.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gwbdfsioo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gveorzmdc.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/glqiflwkk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gxdgzqpir.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gedpontwf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/glaxzscgj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gtlyxftkl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gvqcmhugg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gjqrqefpq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gvjeabcrw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gwgypehla.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gyysblaax.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gziwtcigd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gugnpdgvx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gwfdvuujp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gfjcmdjuc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gzuqratpi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ghbreqziy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/glcnjvzvi.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gclwmddrk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gyjseskue.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gwclwugvc.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gerxvpslz.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gywtljkwf.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gyrdnltms.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/grqaqunxe.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gxpkhrzzy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gtccfoxtn.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gaucrmnmk.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gysxnmpsd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gnhpkljbm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gxmsxxbpv.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gccjaowdg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/grbwihyrq.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/guebjzmyx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/ghutvuaqh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gxjokpadh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/glnoffscw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gsxtpejbm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gucageezz.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gwobsztuf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gavybezmv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gujbtvjlm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gcvhwdlmn.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gswkvdbip.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gjkvyyxdi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gmujttruo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gesoumtrj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gpbqpustf.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/ggwkiijhj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/goeptstaz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gcvtrbbje.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/glcccuqyg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/glgjxjwfg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gcaghohiz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gmxslcjnb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/graukahuu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gmfncydin.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gcjmfdnla.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gofmcqmta.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gtkwavure.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/guocwklse.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gsaoiqabd.sHtML


<!-- 参考信息 -->