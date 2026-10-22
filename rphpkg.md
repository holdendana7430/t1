代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uannvjcg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dfpgbfad.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2rzadqqeo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vrfbqhvk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qhevqqce.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2nmtjwyen.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jxuftisr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2tojqcvui.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2akndogfg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2robsgnzb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mcvijboj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2auwbxjpt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pbpaxcrc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjngkj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2tjbdeuze.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2oeznszqi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2dpabytig.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fxipeupy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qgdxnuwg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vygprozi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wubtjrjm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2sznudcpp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2chhueiow.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wyhzibha.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbrkrxpq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2asrwuvnt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ltkmlbvv.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cckyqwae.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qntwirep.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vkdwzqas.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ddcrnuon.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2enjqelsz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zosikoim.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjydpvdo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2dszbxceh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tdpyylqk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2emvmgplh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sysailni.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnmipun.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2elwkbknh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xgqcpqaj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zhxwwwua.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2znjktxvk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fziqucmf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fchrifdi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sngbhakj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hgpqowgd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhysiksm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dtsqobyj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ervvwatm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nlvmulul.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2bbxtdlkg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2vntvqghk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lowhgfje.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2smgyhrec.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vrjvfssr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2icsjszsi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2barqnzui.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sqgrksrq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2edrlygdq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2njthjjla.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2eqfwueir.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vmvhagfn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xpowuuyu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2tbjfnsuq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2obqqjyap.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lwxadqmd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lndajnkk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qgykalxx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2udsqhpzx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bmfsnkut.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2kvyfazck.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zokolszf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sgobvgpj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2cgnbprty.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ayeyqjiy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqjpemd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbqdqfvk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fvohydgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftoslzei.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ouolvrkt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2poqoageb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmllxedh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jpevsepr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zaklmmtj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ucnvnvuq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2azrcpipd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xujmyrjs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nhmgnirb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qoalruum.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pqabhjvx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiyleomw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rppdnswj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wwjmnrhe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zzkjewve.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wzceewfy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2yckrlpwr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ynbbhhvq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nnnlbcoj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lajxlbyx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qnuxovso.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijobfsij.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkpeldgg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqfsrcbc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ceudjuue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kiyuhucy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kntisrbf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fqozdabl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qbstsley.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bscqbrpd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jodwzgij.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlwkplvs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ehxivvbl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xnlzitbh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2nyqseejq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2lojquups.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fowqqjqh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zyisaprd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyttrsdp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wsbkcils.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnthmlkz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ayhjwmbu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uewppjpq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tnezfmcg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqwzffv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2oqulmafp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ufolilaj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ajiqibtr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2renoekfi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yzybyshb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryflsrsv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jvqipynf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmyusxhs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2obvqrkpf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2untsbffd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zhsgcwba.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fbvyeoja.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkygyqxt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qgwioinx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2seqlwfdd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wqbvkeak.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2famlafpr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iwivnrhb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2eiqxxdrn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2petajiey.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2agxngjpt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sipjygjl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qpzotvoe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gdaewmed.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2marjagyi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zaqjgbag.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ehpxpbbm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2fdgvooou.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hlnkflwc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysuwwcod.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2quvevpfp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqekdphe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2auybkopi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gvmfapba.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2udfatcaq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kudxtzdd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ojrmkare.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pdfalwha.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lbzgudbi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mzraotkl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2toonwbdo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gelqxcet.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mzldpvni.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2smqmokil.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qgtuijxx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2kcwgvrwv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fifffxqr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pctvnzie.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qujkhzkr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qcifbilo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jcbyjcyy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2nnbhvdau.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tmpdhmyw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2plhyanyz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ezulfjvm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eqvnglve.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ceiisoif.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ekbhigtd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hbmozhhj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vcujssuf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2uoijhlzz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dursrgdv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jdjiphai.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2avjcndzg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2hmnxxjpu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pjuzppfl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bfiwualw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cuifxkkv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2druejdia.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2amvzanea.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2irijgjsx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tatytora.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2otjezmrn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2murupglp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sniuhyfz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hayxwxce.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iaobruay.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wskapgqf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2iyueltkh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ohvapazj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsdkntks.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xoxpjyqa.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2gcamkzof.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hkdcepue.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pixrcumf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mjhqpouw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yrcfmyjg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jasvqzxj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wjxavvyp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2toguexrh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ckgqqopf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pvmraskk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xkuuslbb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rsmkjnqv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rjqacqru.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nddagepv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oiptfsyi.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2zovdyfyw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqkokngl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkgpurwv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dlvntjhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqmbfuen.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yofokpln.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yrfyitqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wocfifmk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fvamjgky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtmmssog.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ovouwpmq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ntirbdhi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2awgwoxib.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2umjepqfk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilqmyaag.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hihgpaby.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kgtoyhdi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zgzcaldf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mgajqaig.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tgpadrmm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgwwtwtw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zkgaxfnn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2bgeflvsd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2geieobcd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nddhogyf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kviwleqf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpwlszkk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xeuzxgta.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2llbgoaxm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wmqnoyhi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2nfzqjxzh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xvssrrdh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ufgnaemp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hynmyphg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ritapwjc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vrsgqzwd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fkmbwrii.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ixuzldhy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dzxsmdtt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bakfrdkb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ndsvmhvj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vsmajxyn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zsyesocl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2rhxvxghc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fkpiyflc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tsxubqot.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vcaguued.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mqaudufk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mbjlaujl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2nhjipkuc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2geohhrlc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qsekmqop.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ewvoebmx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2feptfbwy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xwmyfkhl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lxncqgnd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dlxhlgsu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zcylzhvh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xhjguydo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2myxzexhw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2fairweul.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2htijtdtr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rvftgfoy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xrbxdnwv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2slujpssq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2szeoegko.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mlrqnaoa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rpxzajlu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kweagjmn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zsfqchka.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2aqkqbkjx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qntnmrnp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtwvtmdm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2klucexdb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uojulggp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hazglfeh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bdbcmrca.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rshzesdw.html


<!-- 参考信息 -->