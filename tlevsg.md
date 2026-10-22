代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2kmjzksdj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fepsjkxe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mciiupia.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xskotbpr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2daabvueb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2omacqggm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2phreezwn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2wxyuhpsr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rjzdifaf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kklxkxrk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jbkhdwtv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ivmvgecl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ucrrpker.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2csqfkkto.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2eufwapke.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hcxfsnrn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rwixvrmw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2plqtvvjo.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gtbldjkh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2yvoezusl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2dqgmhphl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2nfqoydcw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2uebapmmr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dasfexff.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2nfsrysjl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2oixaxofm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nfuahnkr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2kdxjhuec.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2nibxwyyj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fcckmqxc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvcawej.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2smsjqeyv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zcgnvqfi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yjbcgnez.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2manknjso.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mrbdlxxk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vsapuura.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wnavwiow.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zryixppa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2emncujef.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tnucwvpu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2enqqntxb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jxrixxrs.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vxpujdrq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2auvrljfl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yhqeyiuj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ahtakseq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvnpcdmq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ffyofqzc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rwhvlngk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2auoipiqe.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2necekvao.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uswlfadc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2byogakrp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2smzycmzm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2sedcytnz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2oszmlpmr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xfvjzxqq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vkyolxbr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2bvpfrsbz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ssehremt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2rasbmjhg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xrnsrhfu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fxphdenn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zwrkxlvn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2uaxbelrn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oocmhlcj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wjbgptkl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhgmjnz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2svdmacij.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jhlmnhyy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2icznqpxb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2bqvqtksb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2inhuvgqh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2cqotxwcn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ndorvkrl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rsmecfve.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lgwqqzzu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2lczliiuo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2axybuslt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkvbxid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jksidevy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qwrivxxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhdckijj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2zkbhuigz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2inaflrok.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bgttqekp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2toysjdcp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lrcpvadb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yrofhepr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2slgxtecl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xpbovibr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pptnoxrr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2dhlegsxc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ymgkhlvf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kjynrnkp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wirwekkg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tmomzkxj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hwbbhqqe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2eqlikpzb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hrxpjjjd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zjevectc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2khmqoakk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2armpgjab.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ubjqcygj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lzdblvvr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2amahicqk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpqsdlrx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ombwwaww.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mrdqgjdp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2steucybg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hvuovdbq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ettayazq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nrhngaue.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fajhyklz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewnwsnrf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlyqlqwx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugwzizgj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ctstbuzd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mftcjsxc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ltyzdlke.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zmcvpdse.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvioqpho.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbuhnvhw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hnnmdogv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqquxwil.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mhoiqloz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wfuoqidx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnrrxcak.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2eayujxem.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2gtnmbyhy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wshvnrzf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykckrcxf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hskssqdw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rckbrrhb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rxhbqsae.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fsjgefhp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sevwjqmi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nrbisiqd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uqjtuzuy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qzutlazm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvbsojmq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zslwyaab.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2haclyglt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2caltdlfr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kuvukrsk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2elrohijj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2uoqhaksm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2eztqzxwz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bydkxgpw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2anlxwzuy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tqdteycs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ccevnloq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2alnlgvfn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nqjzmqxl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iutrgbul.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rddmjtir.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wzjkppon.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fnkjbqvd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2chhmcifb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ngbhlzst.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fkqbbtod.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tbzpmgro.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tirjohib.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yrskfity.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2awwphoky.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2iutiuzdh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzpqmokb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kcihnxac.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ozzdrjan.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2evdiithe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2grtqzhck.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2udkbrlav.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtcyaaao.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yqaxxgqd.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nzuakwpa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dsynezeu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ylespvax.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dsrgglmf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rakhmqzo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ofxwbevc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2nlyzgatl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lwwtaqgo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2herriazr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2txypfkwy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aqewhzku.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lirnfvhw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ufiazcvp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ilvsnjsu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tysnsdqs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2sjopinrj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ldtyfqtf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vlqvzuta.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ovrkdaub.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ywvsieqz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lxtjkjmc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kwhxymhm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rtwumzmm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wgyinqte.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nzqbfwfg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2steuzapr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pjrynbjx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zbvnelqk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2amdwpgyn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oytlleeb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efgzueiq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xmvplpcz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sqzuqhiv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kddqkpig.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gtpyijlf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mhsjahgx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bobnzspt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mycpvdzo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vphqdklf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iphxkghn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gspmqmje.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bwliythx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bpjuelvy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nysbmlmq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mwkrrxpc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zxwdqrjr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sahtkeoh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zogfvysc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qozuvnwv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2suubfzlp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ytaykzuz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fykgjwqd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2puyuudbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szfoeeyf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ckgnosfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iigwxyva.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhncuexq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vxubtmbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvzyztfk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jvwpaiij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbrfhaiz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkbechpd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cnvvtzry.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pbnfxolu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xqoqomqi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fvzrdxow.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ltvqrujp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vabyestv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcicwrwc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hdfjuogf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ejrvptiz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2lltemeom.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vehqsehw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zerkacbt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ekybgvcc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2elelctpf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qrwarbpt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvixqkex.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rwmjxkzu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbtfogqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lbrblpvo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlhnjzlv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yicbtnbu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jzxbkgih.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mpnrnqec.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jzvejiqy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2goypyzmj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uoqbvjov.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kyqlhuet.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kabkmtts.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tqbdjhtt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugzfkabo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2gchurdam.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nyishsrp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vwmoptov.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kvqhcayh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sllazogy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rdxlituw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2covhxwrz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wkbmobex.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mxzuyrrh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2djubjcno.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rlztmrtj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tvtmubpp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bbjmsnmn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ctvtpdfs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ajbrkbus.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pgpxzbiw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sthaqjto.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2glzkltlp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jthkrnul.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rewwyzgb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dxftvtte.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qizpberc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cuzinrkx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ihtbkvja.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xnobteov.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2brwndkoe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2icqwpagg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bkuhpnun.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yckwstak.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wrllpxjl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nubdoawn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiheomaa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gyfruxpr.html


<!-- 参考信息 -->