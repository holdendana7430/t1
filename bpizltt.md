代发 wailian999

C#:   (int)'A'; (char)65
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmgppzgf.sHtML

[A19] 交换两个变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzcqsioxt.sHtML

Py:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/ganekxcoc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/gwlxlulrk.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmlkxsjj.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gqpfbaxqw.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjklvvbyy.sHtML

Go:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbrlabe.sHtML

Ruby: a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjhascpc.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbvdnshc.sHtML

[A20] 读取标准输入
来源：http://read.share.fanxiaobao.xyz/Article/details/geieuxmfd.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glealrqpn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fanxiaobao.xyz/Article/details/ggqvzsrmz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fanxiaobao.xyz/Article/details/gisbivjra.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwyzzwwz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fanxiaobao.xyz/Article/details/gydojfqtj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvcgcmjr.sHtML

Ruby: gets.chomp
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcpkjqxv.sHtML

C#:   Console.ReadLine();
来源：http://3g.fanxiaobao.xyz/Article/details/gjstivjzq.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griepyvtd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxpexludq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuzcrent.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzeqeknd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghpnrxfeu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxhimeco.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fanxiaobao.xyz/Article/details/gdfvzpkta.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbsvpskx.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhynbsp.sHtML

[A22] 获取字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxvoyfdcz.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxaulahg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fanxiaobao.xyz/Article/details/gaskclaiv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkpeqccz.sHtML

TS:   s.length
来源：http://3g.fanxiaobao.xyz/Article/details/goktaguzg.sHtML

Java: s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhpqvqgx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtnmxvue.sHtML

Ruby: s.length
来源：http://baike.fanxiaobao.xyz/Article/details/ggkcmlnfa.sHtML

C#:   s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyuldkpv.sHtML

[A23] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhhymnmw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gxjnyzbcp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gedabzohl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaahavtnc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gehymigft.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/gcpxfnlvu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gobrzkboz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckhlimov.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/glfeoegmx.sHtML

[A24] 去除首尾空白
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhwdblkn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvlisymh.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmivhitp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitktuoiu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gptbekrnj.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fanxiaobao.xyz/Article/details/gusxqofdi.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxrybdcp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdzzwzm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gpguqisps.sHtML

[A25] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/geveupriq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fanxiaobao.xyz/Article/details/gqftvnnpt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpacaofjh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcajhasc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqbqsdxq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwybqahg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/grjgjyhdi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyizuuvrz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwjzjklz.sHtML

[A26] 类型转换总览
来源：http://baike.fanxiaobao.xyz/Article/details/grvsittrv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/gfstoqgfq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiiabkbd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjslcxbp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fanxiaobao.xyz/Article/details/gviobcgem.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjufqpcrq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbmwmmwx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbrieoy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fanxiaobao.xyz/Article/details/goqvbdwdj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/greglmguy.sHtML

B. 流程控制
来源：http://blog.fanxiaobao.xyz/Article/details/gtyeszfws.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmlsvlogn.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjjgrqfl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gebnuwhth.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzjmoqvet.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gxblieeor.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcuqokrz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gphobkqaz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdhfplaj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamiopznb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gxbiuqdmw.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbcbjogo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhnvwlv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqaytfkg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfmcueqb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtypmfeuj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuvshstf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrhwokyg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvpkswij.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gfuaoeyjz.sHtML

[B03] switch / match / case
来源：http://wap.fanxiaobao.xyz/Article/details/genxqeqms.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fanxiaobao.xyz/Article/details/gktbdkash.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guezqftee.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ginfwvwda.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzgsnfvlb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiyhcyhh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcooqamiu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fanxiaobao.xyz/Article/details/gjtzjcdfe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuvfkgyl.sHtML

[B04] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyeknpwdj.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyxgtihd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzblxhnwz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxclwmghs.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghvbectcx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grxgjjigr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/gbchaeurw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqvkgzdj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzrwqusui.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gcqzdmdrb.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcifqyks.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghmatmctz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gunydzwxw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gugmyxgwn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gpidwzwid.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fanxiaobao.xyz/Article/details/grhqhhcia.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrbamjyw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisnxgxnk.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqmtlfmv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsdexizr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfzbzceoz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gagozfjpc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gcnlknmzk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijwyembd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gakgebaez.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gfdnxaonh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gaufmdunm.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlavkrwz.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gbdasbspc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbbcofco.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glldqcbpw.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gexhfpyri.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoevsgqd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gqebjrtoq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxedupmr.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxleepzwq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjspytvtz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynezunfl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkjbkntk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gcuybgahe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/glpztexra.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/geetrpnug.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/ganrxcmgm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fanxiaobao.xyz/Article/details/gyifohhwe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/guppcvycf.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gjktywcbv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/goracifdx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gauguxukc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjydjspdo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvcvgrdd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gegpywsub.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gzjdtzvmo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gprcucbdf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpcirrjod.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fanxiaobao.xyz/Article/details/glexcytde.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfsopzgt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmftqgwfg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzgwnhtx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gjxlrrvar.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjpxoqile.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeeiegud.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/guvkiazfw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlinvylw.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpiftbau.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gytpmvqzl.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gxfrbkhva.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjbhdovd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvhkegjw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpydosafm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fanxiaobao.xyz/Article/details/grhextxlm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgrwravi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gqtshkhua.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gcolypdzn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswavnrm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/grxiekxpo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gxdmxhgii.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcidghaya.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmwqisbe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgcpmbip.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/gtrassxus.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwyuqfeo.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gtszbselg.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/gcnhcumpi.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gyhjxcrds.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gerhpuepc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgizagvp.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbvxadnt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gdvebensx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fanxiaobao.xyz/Article/details/gbfgyqaft.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsobrjtq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjculfq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsazzyfix.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqncdirmy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikclyrnr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnggmybuv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/geyktoawm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfuzyfwwj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiwntiin.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxionblx.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfhxqbls.sHtML

Py:   a and b or not c
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvfdfzir.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkcesjy.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkjichjc.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgjrxyzu.sHtML

Java: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/glacidqyq.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczdwlpcv.sHtML

Ruby: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gkntmsifn.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gitebdkiz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gftmfyzta.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlatynxf.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfjylqpeu.sHtML

JS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gpeughaer.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gjshfwpjj.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gzxfsiqts.sHtML

Go:   if data == nil { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gzsvryknt.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvowhwwf.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/glyptzvri.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gullupotm.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtifxqcu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgtjxhbz.sHtML

[C01] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbdbclxw.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gdcqtmyob.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqgxluxa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcgfgxdcx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/godayfoat.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnexvkwiv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdwabrdx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkspjsaxo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbdzzmw.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwxgqxkq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gbowaamrx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqijbgbq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjxozcgwo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjglxmtis.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqapfdvy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fanxiaobao.xyz/Article/details/gazihkwkr.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsgtvdmv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbvhfgjn.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjqwlpvf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwdxdkho.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmdjaofzl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gncwwksrm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gudbmibjq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqtlofooq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fanxiaobao.xyz/Article/details/guunsobms.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/grvwvkgfd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaijatym.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzmmfoeh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkdivfgw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gufvxhscs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjktkgz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvxopjza.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpzmowvt.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzshdfwxy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gztzulvya.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgnliozn.sHtML

[C05] 返回多个值
来源：http://wap.fanxiaobao.xyz/Article/details/gthktcycn.sHtML

Py:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gauouvmvh.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gcwzrnbby.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpczetiw.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/glzznfwvg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnshmneh.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokcmjyap.sHtML

Ruby: return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgddjund.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyzwggaw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtwdiams.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/goafmvqrf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fanxiaobao.xyz/Article/details/gzpkgdppz.sHtML

JS:   const square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gxsvheybc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhllghni.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhdwjqya.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/ghmacnzca.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplsxemhw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyshfnay.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqcgssb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkddfjni.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gtwewgayp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/ghxnaxqev.sHtML

TS:   arr.map(String)
来源：http://baike.fanxiaobao.xyz/Article/details/gumhmjodx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtwwkehy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/gjkfcvvum.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gsqqvldgw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fanxiaobao.xyz/Article/details/gxrbbglsy.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gdzqvkwuy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gcchkynyt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbicztviy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnyxpzfy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnfwglnqk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fanxiaobao.xyz/Article/details/gpedvtmcl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/geedhkjft.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fanxiaobao.xyz/Article/details/gkiwspwwj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghotqdatx.sHtML

[C09] 递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galbidsfe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmiwaggn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmuastdie.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/guosdngss.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/giertwpsq.sHtML


<!-- 参考信息 -->