代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gzpkbgpdn.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.zdbjq.cn/Article/details/gswxslwjl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fehbvm.com/Article/details/guuealigi.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/ggjfyankk.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gktbyotka.sHtML

[A19] 交换两个变量
来源：http://www.blog.zdbjq.cn/Article/details/gtckowoim.sHtML

Py:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gqvsxjxcu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gtpfbbvbe.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/ghygbjftz.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gfuqbitqc.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gkfctmdlg.sHtML

Go:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gkjvdtnfo.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/ghvljrcsn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gciaarrwe.sHtML

[A20] 读取标准输入
来源：http://blog.fehbvm.com/Article/details/gkqdofejm.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gmmryuwkj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.hesvh.cn/Article/details/gmyxlokvf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.fehbvm.com/Article/details/gyspweaoi.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gaaiboutp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gewexutam.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.hesvh.cn/Article/details/gzsjkkoky.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gehexcgvr.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fehbvm.com/Article/details/gnfqntkdf.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/geznlvhcx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gsefpmugy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gzzpjmnmg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/ggmnhfbxb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gqjmfdlfa.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gdeluegjb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gvpycqpbi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gkzezujxi.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gzybgifyp.sHtML

[A22] 获取字符串长度
来源：http://read.share.fehbvm.com/Article/details/gtsymrnrl.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gddnpdxoc.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gszbegxmd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/gxreekevg.sHtML

TS:   s.length
来源：http://mobile.hesvh.cn/Article/details/gjmhmqfro.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gxfruyqnw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fehbvm.com/Article/details/gnqhsjtjd.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gawqlprny.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gptntpzjk.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gthubzmvb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/grxzdbvya.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gnfrkxqly.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gsrjqynwb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gakriqrnc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gxagdnvfm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gtvqmvvxz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gpysibseb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/guoqelubj.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/ggxnpshjt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/gllgrxpuf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gunaestgo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gzvwgikiu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gnyfdggyy.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.hesvh.cn/Article/details/gmirrmpyp.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.zdbjq.cn/Article/details/gxkjcmnpi.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gpjscgfkj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkrgysqdj.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gaefqikbe.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gpxeqkhwj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/geijnrluv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gfktpaxdp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gdwwvbjmv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/gzfjhwlmh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gracflxbn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gmdnjanvt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/gcaiodcdx.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gotcnibyi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gjsfheuci.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/glkllzbpl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/gbakettop.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.zdbjq.cn/Article/details/grmuhvofu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gfxpkbwvw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fehbvm.com/Article/details/gjyqhzjfe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.hesvh.cn/Article/details/gmhmftxic.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gbajkfohf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gypxhqrnc.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/ggofqcjoy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guobzzosw.sHtML

[B01] 条件判断 if / else
来源：http://wap.zdbjq.cn/Article/details/gujuhwrje.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gflezaqik.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/goasprkdu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/ggpaiyneo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/giyaoekhs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gbgicymij.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/goemojahq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gikhfglsv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gtubtpvso.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.zdbjq.cn/Article/details/gmlylrloo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gilnxvvtr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gyuiqaxkc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gbmartcao.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gtxscpozr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gfgojsduk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gmegefbir.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gjhdehsqw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/giwodkggb.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/gmcxfzziv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.zdbjq.cn/Article/details/guslawieb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gcvsucfpi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gdbmptvdx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gbyvofzjs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gohwispbu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gryhmlrpm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gujwhozsu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.hesvh.cn/Article/details/glzankesp.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gnblkdmrv.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gmmkztlco.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gaoxnnisb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gahavrhdw.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gzfsygqzw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gpnzgeiik.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/ghteuexyl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gwtolxmia.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gycdmwymk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ghiubipxo.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gqzvtcmtr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gwpqcenkq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gniifxyox.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gppihcedo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gdryjllod.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gcdmeldul.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gqiyviyum.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/ghtzlomct.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/geipkwpaw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gwweznylj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gdocpbjva.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gkhofogqb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gmwbhkawm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/ggswrivqt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gdbxrotqp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gzfjhosyq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gmiynmyaa.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gybhwjjtu.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/ggcuvhlln.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqcdoukh.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gtnzwhiot.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gbkipgzak.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/getstdbio.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gzqczwzre.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gkptaypzy.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gsgdqbngp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/ghdgklqps.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/gwpxompka.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/giwisvgqz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gynglhoyt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gdwjloomz.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvxunaclo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gkrcdpfur.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/ghgromohl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gtdbchnaz.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gojxdqmul.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gmakpzykj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gumjyfclr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ggzcicegv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gedmoytiv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gynskzwce.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gdtlzfgve.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gfvdlnpci.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gybuqiulq.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/grzuqxxbp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gbmpolkqa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gflulxfcc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/grzyyzdkz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gublheobz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gioltkilw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gzdqdomxs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gcazgdorz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gfpoxoijj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gbghdembp.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/ghpspznyk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gxwqpqgql.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/ggbrxisol.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gecheynsc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/ghclslacs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/girhzjaco.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gzzhsggdh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gmclmxyfn.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gjapmyczo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gfrtfcwmr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gpfotyprt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/grgmdvmhs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ghmcegiko.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gzfjnviov.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/ggghurwxr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gkrdpcjcz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/glgcucmij.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/giwujkxeu.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gybqbfyhy.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gqeavyxgk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gfdxiluic.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gnxeuxhbj.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/gfsazfkah.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gruyuedkf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gettzpdfi.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gbviawlvc.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gpewzwltg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gsakiuggi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gywtspvdt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/ghyogohhq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gziwuzjhh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwbxfpcw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gyxeuzpzl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gjnxsuoml.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gqdmjsmhw.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gwrbdvnhi.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gnxvwrghx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/ggbqmarda.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gkopkqihs.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gweikyeke.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjgkfzwim.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gduugdisy.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gvxhqlztu.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gpakxnoin.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gbuipbxxv.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gdfvxmnnd.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/ginioukio.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gpusvlwuk.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/giqewnpxg.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gdqktkcbv.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gkaiufqab.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gxjsckfag.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gxwslacdu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpergrxyg.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gizdgpjxg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcegsjuub.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gkqfpsllt.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gkorcdbph.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gronbvwrq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsyldfkbx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnsouhqhe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/guuujkkjk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gcczrlyvl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gfijkaueo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gsnevgowr.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/glljcixtg.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gqmeaiuwd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gzopynebe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gubryddjc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gordpkuoj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gzegkdjuz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gkyvkvdrq.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/goyltjgmg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gomwwykqd.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gvkyzbuxc.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gqvkvnpbe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gucxvnels.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gkswadmih.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gkyfyjqvy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gyavgwtvh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gixxabzwc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gnexkonqc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gdiyhzwzs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gnoadmucw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gmgpixvly.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gybxnzagd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gylydjlwh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/glnbkycyg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gascvfbkc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gggawnvgx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gposcmynm.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/grzatrndz.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gcgsiysvr.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/ggprphzpt.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/genzqouuy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gpdvfitzu.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gpfcovugx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gkhbbblqc.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gcqkoruhc.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gkgrwgfml.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gmruqrdvy.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gvxumjpmd.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gbpmkkciz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/ggygqopms.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gfyctzdej.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gutvqipsm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/ghdxzwukp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gsfvkqjta.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gopcikbmu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gzfjzmzrl.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gfxwpmxpa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/goupbobhb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtrabuhcn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/giasvfquk.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gykyabxku.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gneyxdnij.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/ghlsielvb.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gnwfdrvsp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gvuhlnzcx.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/ghehwosxu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/geuvvnaxb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gijefvnjc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gdhfcqxkg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gpdjlxunx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/guftswjnt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gtsfecoon.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gpwxfacta.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gmalbnvpm.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gyvpdtwzb.sHtML


<!-- 参考信息 -->