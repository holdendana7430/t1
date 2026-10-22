代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jwmlqxsv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ysquzmmt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2nacthurk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ijgphogi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ebdtzvbo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2iinggvlz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tqdjqfbv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2skcaravp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mqwxlwpb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pbmrmflo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cyfaqepz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ffgzbeym.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2iyqiviym.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zlotufek.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jjgoatrn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nielwvae.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2egicblfm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2oluaylru.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nufmtgpz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xykeyxqt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2slpmgpwy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ykcmoumh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2suxhgwes.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xuafsvlc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vpfxhguo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iuiqrnna.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrgemlen.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rbpylwxu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2enyvuxof.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lqhrojkn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hbokgmtp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2sfslvagr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2psmxczue.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2adipgtum.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2quohqpjy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xhddfoxv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2epgihxqs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fkmkvbrg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nypllzjr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iyndhyzd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lrvaesjp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2exkkztpg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2giqvwkrq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnyttqit.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pplerdlq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2iohugfqr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vrkdrcux.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpyuicf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wzlyoftd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2uybvkyzj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mszjweso.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2pwnwjqmy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtahnkrz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qbfqnigr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2djzijncd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2iypaohwc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwknuhya.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hdwawvbu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ygnhndwt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nvsxbtgg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2plkyuicb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2htiyittf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jmqqpwlu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rnnptjmn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2clletcvf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oozakfbd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2jalgsypw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2frxymsws.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qvomzscq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fvubtqkz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2farrwxxb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qlxmhxmq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2imthimxl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ekdktvbd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jqnebebc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2goktwjcc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2brialzju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqpxiopy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2cveoykgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtlqbuav.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mkoixhaa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2utthhdma.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2sscmmylp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2omsecxaz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tdlgwbnn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mzwgokbm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2opbksvac.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bbuebdhu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wgqjnnhy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2caguyrhz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2vuquzzgp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2aefpmcbz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2exuviqpc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wcobrvbu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pfhcqonc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pstzyonj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jwsnqcyy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pgtqpfdw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wauhjbtl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wapbxxsz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fspbcupv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufhewurh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kfvdjrpg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djcdoabh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2asyqtejb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zwlabvyd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bsftyypy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pgtbfbva.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2duxvowqa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zjscbysj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zpwzrnhq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpxwbije.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2heehaisg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2uasrvail.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fnpfvgal.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2lumibsvg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ickzuvbp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbistre.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2uzrdlacj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yxpnxink.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kftqltlq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zwnozsyd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hkddaxib.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ziyuzxnt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2luafwyqc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vnlbhgfh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gwfipmwl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lwflkjzu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvopihoi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2porxqojf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xceibpne.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gurskgak.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2vqzcoily.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ffucvnhi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xhgoldsm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dmojtvgm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2helrylvt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eiwzdwdn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vattphrr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cedzdhrn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kxhupreo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qglyprdr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nucacyqg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ywtdwqrd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hdpkbelm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uwjyygxf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ogrmfrts.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ylukjteb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tsegregb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cagjjfbe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2btsfqgkp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qysnbvvl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cstlbdgl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wudzqrod.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwclqjdd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bgczwtyd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yaskxuey.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqbiiqqq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2avetawxc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tasbcwom.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2imggskbq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2kkhfufyr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nfssjnah.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jawjrzsc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ncdpcvfn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qpicgznz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2txgvprzx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zixasyvz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vcicjruw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mmcjmvwy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zrisrvpf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qsletaas.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2heodkoyz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ozdazfzl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yncclkka.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lenbtkyy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bqvysgfm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vampwowk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sclauybw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykfavmal.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zcmexrpv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2forjjvdz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qmtrscza.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gjabbxci.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mitjotdr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cqfdrcjb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nisjijva.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2njmvbksa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mifklhno.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mdhtuccs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bajlxsjl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzlwkgb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rofvogiq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bvhwqmmu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2putzview.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qnkwznvi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jysfzdbc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gxdcocju.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2aheeqqox.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxrlpif.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iqqptdgs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bkxrzybz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2liratzwo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yblheicu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gyaiuwbe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nienjtyh.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2akxslust.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qbulqigr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ejzdlqpu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nobqzvzf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cewxwupu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rnmrzlep.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2izdkkrza.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xtrlmedy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xdkuwwrh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gsybxccd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rdxmfooj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tahhgfty.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hkfbqopj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kltixbgm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qfsdpmty.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wndtyglr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wfimxiss.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fgvyflji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uaovrcuv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iczqjfva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orwlhksh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwkofwtd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rfpabnkx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2adlhujpm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gmofspyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2paxblhtg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xamvenof.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zsinsxdu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gemtxabz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbfcvelc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nxqvcctl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hibgwvzs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onwnqzap.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mohdsvam.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2incwfpjg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ewcetirm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wdbzferm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jybibazc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2eprlnfso.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ngtdebuw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rpnqnprw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2imuabbvc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zjvzjrqz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lnzsuayc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2okbjwygb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bxxyusgu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqphtwco.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rtbgbytk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mouzdxvz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wwkxpfcf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lwgtfhhh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mdduqvgl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qagzkfjv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fdkmcwty.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lzbndppz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yhoqaxrc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2plavphqt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2tvklvcow.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qojqgolv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2enxvvjld.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kufltnlf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qebjllag.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dklllzpy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2czlzzxgv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wuptvvih.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lfvprxzl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mvvyfkrk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2furdvsks.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2feupcqye.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lhywtobn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2csfbzkbu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xodqwmee.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ekavyxvb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ceyrxdhq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yvljbcmi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hkvnyzqz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmmrnbl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oaobxfrw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cgtcuhmj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ocgxufjh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zamyjzwo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bnjwiwcg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fahgfbye.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vwjtlrau.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wirxthky.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ozzmzbfn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2igmghvyv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzqqkmnn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mfzcgbbj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cwbkdqha.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rrnybkrx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wruojiqs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2scnzadgu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cdwseltx.html


<!-- 参考信息 -->