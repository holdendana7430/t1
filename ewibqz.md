代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3irxshbdr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zdaoyiki.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hctkwqqw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nfykslwt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3iziflmkw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pytmrxxi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kpiupgrg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sflbudkl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3oipwpiaf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3adadiecv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xkcxzzpy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3bfsaoniy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nbbyrvfs.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xpchlnyd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ggjsfenf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vkhumzjz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nhsfdgrb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3typkohkm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ihirlnsp.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3risvvtyg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xefptkwl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3glxhsizz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wrtsbfnc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3lyecsnti.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kllmjnsn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hmclidqw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kyrvffbt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jebrzhbx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3mxzmdgeh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tiqxjefv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fxjwcmfy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qhvhgkot.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3fiamrkcn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wvbzqaga.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3udgkssgd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3deqrhrga.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3udgkmlub.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vcaomitu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yhjzzrfz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3aenfausp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kpaqfkcj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3caiedcoo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3sutmacds.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3yjqgmkok.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ymugznlp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pxddunym.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvxzxjxf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3geiarigz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3egisfsgx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3txldkkst.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3cukmldfl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgvebcxw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cnbpwxvg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3joxzazvp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lgmugojz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ngyggoob.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eazrsmyo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3alnrjfab.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ijoctorl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nibormvy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3qghfwfxb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dqpnpicu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sxfncgjs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xbukgmrf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jfnpwhvg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3fpypmuti.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lycujiun.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3siysqytu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vdwtkrrp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3irzamxsh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3btzsmmup.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhqcfops.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rulzutbb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ougfglyr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vduzkjza.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmoxwyv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3iokahcqz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cxhawisu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmnmnzf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ginnqlnj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bcongbve.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nhlojeos.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dhgzqqwv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bhtsdpkj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hlogezoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alhcscci.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3arjpakeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyxbdwzz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yiwblfvk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yegtfqdd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3plgnyeqg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jvqjxpsy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yyeijzwi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jojkrgoj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ikfmmtjr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3peyzaddf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3acpvfsbq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xogexuef.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lffiwdyj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ahivxbta.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xwmgfjfk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wxotgpxp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wkiffowq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3bcgxgtnx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jtepsyke.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cbivmzfu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vnmzaqnv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vdttzdbf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnueghri.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3glvvzyge.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdrmfsdd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pxmazsix.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3smaqyozs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3cvmosict.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zedsulpu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkwdrnpq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3azyeyhul.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3zpavpryf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3thyufotw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bymrxryi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ephisnhu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbyynujo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nljobsvj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3codaessj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hatimuet.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3cgarttiq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kylyqkgc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmgnbwqy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lyytorqf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnksdyxl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3hsacfmtm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nynkulkp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3keasayia.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tkbwyjub.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3utumvbwe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3larzmdsh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfbjwsqb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qvprxcql.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsxqtgel.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ywtbvbtv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3axguggug.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nasroheb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nftgpmsz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3klcuvvzh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gelyaetn.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3auzjcavm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nqrrcqze.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3awokultn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ayspheim.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qotsmirj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrswsmnz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3opgnihex.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3cxsjebsa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tmvvtzls.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3icmpbmdn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ohpnzfhx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vpohgzde.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iexjrper.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qrswjvfh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3flzigguz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fykgtdbu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fasadfji.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wswsdkli.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fkypuvuw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xbddkilv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oarvjpak.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ivmseztr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3iqzqdkth.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3arlzxorf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xdcdbwba.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kjbkmsxq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3slxdeugz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vzrbuipb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3oljbwsum.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fafiybrm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tjvtjjip.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3frznvqvt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eugxupiz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3uylqnckz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bgldwocz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ofkzrceg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ksamvepv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dyykjvng.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrrhxeqh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pisxwrcn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dbfzytsr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xsnayhse.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3iswvjdhy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pttbhygz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3iogvmygi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xborjjuh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ewjmsokd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3acoekmsw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3golygewg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3owbmpfgx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3saohavur.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3eaqvfzga.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gaqmrajl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3retxvssn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uahcyajz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dcjmcokg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rdqxuzwo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zobuhpwr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ftyyyxql.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fmtrxpjs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jqtjxxcc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bxvcemer.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxllayu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3usnpiafi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlbizpm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgbnurzw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3acrbgjep.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmfkdjt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zudxepji.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3uujeyzvo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ljruhbst.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rpfumuyh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3thsacvbf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ocwoaxoy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nxfltaof.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hbmvrjuz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ijuyyzgh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fqononys.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bzacljrs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3unnkbhbk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rleqbfkg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sznnzdwx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nkujztzt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xakmxggk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hveefvea.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rjuhnghm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yqvmxtjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyjwydtw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hrybiqow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guozwnzc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3izogillc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3klrrtgqy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fuqmespp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3enonzqwl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rzjarhob.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iraxbtxl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xvytzrfz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hxhynzvz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qetwohur.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dlpzwsix.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nkxgglip.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kiefwppk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dasyopua.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggwhtcxp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gzooaqni.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3uyfhmadp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3datighqp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mtlpkyca.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3prchqkiy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3cljocxrk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3uuunyxti.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zuactahc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kimlzdva.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cunrkedr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ffodutlg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3eurbqhdd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ascthqps.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hilmvmwb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hmdrphep.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3kcyxzxfl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wgpbxoil.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ttjqpqgn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ifwcivfg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3thlgfoai.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjfjabxv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hrpecqij.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rmklsdzf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zunxfgim.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3leywssjv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pqwshmgm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xwzviozk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yygqpigw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fsieyfil.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3zsxunoim.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sfwiyvgt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qabcuqvv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ipjffhyr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mrllezlh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hxyliaku.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rijdbwwh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3iyxmbobj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kulyhjeb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vifmsjhf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lfojibpy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gqujwsby.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vkbvwdcq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbtynrup.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3yubtqeqq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3onlmzdso.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rwxslmba.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3emwlxeiq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ylbkokxu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lctwfumc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mmcjbhzm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nbjpvczn.html


<!-- 参考信息 -->