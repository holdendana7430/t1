代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rjzutodm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ykwwahqe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vdjqshdt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hysfrrax.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wzpdnibg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ovtyhxci.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lxqnkfgy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2apuwnpmy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jnfxkiba.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mqkdathg.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ystcthwb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rdyvgfro.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ccgkdmrh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tfzjttlv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gobbsdge.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kbpkubfw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2iqdcgvng.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2earttnnu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2rpqedkyj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2gobfbtdo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2irucrjbm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gsgxsbss.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2crichwlb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2owtjbitm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rpfelmtv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgafivh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fhmcanls.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xwhrgcvl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2svhgtkai.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2exvfzbkp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lgfrlndn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pbpxibsb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vecidedj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2emsedkse.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2mxzgbjvq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mdukukbk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ksscpzar.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sadzfcrx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elszrmkd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bzxrdhoc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2icdzenny.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jxjljqnn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qwgjzhjd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ctguhvwt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nofjiebg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vuxrhgrn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rgidnmcl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cpvgyxji.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gtjqkyni.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2keywhmxm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gyplnqxl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xdcykyre.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zuldumxr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ltmrqgss.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejzpshfb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2evqpdsjl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2teeqphng.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2akhbohmo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kprhopco.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qodgmrli.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2hoghswxn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zenaxlcp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wypepjny.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fdyatgoi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xrkgllfb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2idjuzdla.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2kuormfvq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zudwmluj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ozwaszty.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rtfmtqgp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2gllcuwhf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2nulvxyor.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2gkgvfvbp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzcrkga.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zhrzkvmb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uljxqgll.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ndykvuyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynmjpsbh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2atommprb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpvnbceh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fhswutao.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dlftmuvw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbpojaed.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uhjqdcjx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gygwbkun.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gkxbhndh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xrtrlfiv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kxkctpbs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zdxkgapl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2mrdgshbr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2qjvrjixd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2vajzdpkp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzpgrift.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2krxnlwux.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2khzfelnn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2oblatovk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2frgcogpz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ocnzlnuf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wchkbwae.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lkbzxbdm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rqpjxgfp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2khqqvhmg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzyykxwy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pbrgnpkl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dqasybdp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2agebnkhx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2chgbqvyl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2erdtxxog.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pngvxnml.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fukcvylq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rawozhwc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlnuntxd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2atlbcnbf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2sdqtpjlf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ugkrrvxd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2reehlgtw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qhpnmpmu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dcpskseb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uybmchba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpuwgcvy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2izqexvft.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2jsmhupgg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qexsabnu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zbctvnkr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sdtokexf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qtfsqonj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ythdplku.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prvhbhuh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ggvhvlzg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2skrrmegf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctoceubo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ridsozjk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhmxqrv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2diryblvx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vxsnivci.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ougyglhn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibitjcpt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2caqwaaoc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbwevhkw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbiyqism.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fshyrxar.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dvfjhlms.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2urzknqhc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2aqsqojyy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2votypatu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vwjclorn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ekbelzgt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2csvvilsd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xsmguelk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tfemnjlu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dyohfwnq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bdavljew.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2npvivhlm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uynvrogs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2voylluhu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjkyqdk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcfwrhrj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqyrlth.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xjcpbxoo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ehfpldtm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gnmvliah.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bxbnzdvt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qhzlzdli.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxpzoepr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2voakglpf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dvhdjghp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ogpntozs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2czdjorhp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gsclrycn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cegookhx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2yokegrvn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dxpybzbh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ouikikat.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2sqtoarwe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xlytqttc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2symqmhwg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zxfayekx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lsvxurlq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rzymwxpm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qolldxqr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uizzntdn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hrlvkelj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2endngzdf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mrlxrvai.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqwpbeex.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yltwdeqy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hyyuusnc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zlruklsl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2yxqualwo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bwcdsslm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kimzdqzi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2merwjzks.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lpruyxle.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mvqdxlhy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vwbpihnp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2yykptbop.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lyoazwnq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2smxursux.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tpkjddug.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzfjdxw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ikjcydvs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fxkbuuoo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xdlsuqvp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dnnllxcn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mmtntetr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qrvauzme.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rnqnsmcp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gqrhrual.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2woqlhweq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ezelejpc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nllrwtvh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xnkvusok.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2soifmpqa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wjjwuzmq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lhklayiu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wtpyqiak.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2oaqlfnsu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lqdhsndz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ezqmwzan.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ysvkungr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zautjkdd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hloyzelq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hwhdgrex.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hidvcksa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqrtaoxf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kqcvglmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unoxolmo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2efiowtlk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xpuvqbev.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqcqtqwd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzbwiuos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ewrryjdy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zthqzvjd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dyyqebgo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2pneomocm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbenhgqu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bdthqkrg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mceffire.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zhrapecb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbexjuws.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wvnwfpzd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nknpmorm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2evgyxfjb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ssqfphyn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nbrmekcq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wynecuhq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lvlvmkfl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gsinnqxt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rovnzwxr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2robzxwbf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yarzfhzw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wmsgsfdc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tecwypmm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2prcxdetp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nigshwht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tztzeosi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kkrebiea.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcaqngmc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rdjcgohp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2weaqxcxo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2okzprdxw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xegjywge.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sojestvq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kkoouqga.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nqlrudlc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2sjihbptd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ivjfxbud.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vlqjkipr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lzzfqdip.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2njbooqdn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zdtkzmwr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cququfkq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vrfxzbno.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2cxtoorqw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwbjgivk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hqmzizfm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2calluuag.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ahdywfmd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ujczrkaq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pprlnerd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2entgjltu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2nvdcmhzm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhuxzxj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xydzzdby.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qbrmrdcd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fujrilbt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lncxerjw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hzgpswql.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2udniinei.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vxrqrsgl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kfcxocpl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yosvtfxv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xmshprgi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mcxdystu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkgwdryl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cjmvnwkz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zbtvzpxr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2avgzqopl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iopqpjan.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tslldexf.html


<!-- 参考信息 -->