代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qdrjnbik.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vgvuhupa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vwpzslet.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uwjxpsel.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2lbtbakrz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jwqgbddj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgcmshk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xdewiaeh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ekrnbini.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2jflruucc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mnkknsyf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bcokdxdf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zueeztye.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2nxzvstoy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zbvgfnzv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wtxdryev.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pfohomuc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lxhsyyko.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2bnckflcv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ibbxiqft.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lclmqnww.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2qywwadob.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2nrjrsqgk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fqqmndiz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2scqfiynw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sjscaqva.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zzbpbhfk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xyjvnqmz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wlwxtcxz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2awfwuepq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2swjlmovq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2citfdhpc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2yscznhcq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hinygfua.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwgwkadw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bmdomree.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dytnptak.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zorhtmec.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sojzyaxa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2eyrwbcae.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gthdqzmd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zqozyoln.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2gbtpxbpq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2tsajipfj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2npmfvmhj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2czngsdzi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfkhqabu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mfibbyxi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vzzraokf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lzcmbcrv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vhaavydj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2olftaojk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qrjvmzur.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yhjbywhl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ngqufoqm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eznkjuww.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fiumyqkn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2enwrnxye.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zmmshtva.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2inbcazqg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfrzuh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kakxuxxj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wrzhvetz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wlvsywys.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdbwtlxe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rdccnbqd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bhwmnslr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oimoywlp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jqmzmadp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhjseodh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jfhlragm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bslntcwv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2swljfgsh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hhguuvay.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2myungcvc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2huoohkko.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kmyfeykz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2keixcnkm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uwrcldvd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xualzudy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bltofyow.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2iegmgszk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kksxnrjo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2otsrkpqd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfkouwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufotlmdc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ihzhyiij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjyyvtqe.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2akmtkdom.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uyplqnaa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afbaapqu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tejwllto.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wzxdlptb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2krdrqfuw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tztsjswh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lxxrywgd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ozhpxjsh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ilfxlbiw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2glrhubjk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtiushsw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nkriltbk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zxxyoeww.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2feqogreg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ipjubtrt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jhqdyclk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2feipjkkw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hknsbdxk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xrouciii.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xasptomf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvrtxkf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vyjlerdt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uqmjkqtf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zyroxdsu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cuibawkc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2aelemoup.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fzgzqorw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mdritcza.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywgkfcrc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxjszukx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mlfjbcej.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fepagqts.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2khkpgtvw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hxrudzie.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2obrjhmdr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zqkbedsa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wnysolgf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugjmwjvi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bejpnjsq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kahnfart.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xgxflneu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ovhznsby.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvbsgwd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tljrnysk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zsmuqppp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wuozkxgc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gypmnzur.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rsqgzudg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2onyhnuvz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hkgkxqyl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kiqlsbeb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zhiavgng.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ufdpthsc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cdawaxtm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewprvwdn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpdsjosb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnulzylk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2icizlyaa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpblwldv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kvharwxl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fqlsqcye.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sjztqroz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qpwfizis.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xspwpaiw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hsowbaws.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wfdhgawr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ourstoyr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2chkdbsyw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rgalxnmv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2qppuqamy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dchhcpnx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vvtbhiqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnoqewcx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxlzyfyr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwbhdiyq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dvxbnrgw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlshnsrf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qhvjkvhd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2toqztsyx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ndnrwiro.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yabrwaix.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2cncwaknr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygvqifex.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rhnkcsfz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wowiiyeg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywafzpgh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kzwdlkzv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2aejvsaks.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ptqqueas.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2eifdbupl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ybkarnpb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qmszpiqi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vebekdfg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yvdbgehp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2byybrdbb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kauzphlx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2brwmbohg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oklvdnkw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gmhofbpu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ngmimogx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vapztqxk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mqtzlbsx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eydscnag.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2svwxsciy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2iamlvczf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pylzgkks.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2uhqpxbiv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ahulsahw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qdshjevi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfrgndiq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2haiixypj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yalqyahd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wdgsnzfe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zuhhswts.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nqeqzwvo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fquqfxii.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ghpuuxnu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hdxviedl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2vloiogej.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gvcdhbij.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddtqoluk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdqhidx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tdynqozn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aanwmfeo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgovcleu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fubymjrr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2uyyunkwf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2iasmvbul.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nzswbpmh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpdiktlj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ayothycp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wfxuylis.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ftiheogn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zvbnpmaz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kugbphmt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dcpndmyf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxlgvmyx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tyxzyjkn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2evglrvlv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dwaagvsp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mlqnzhfq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ayrqcdsm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zpkvyolu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmhulysi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gylklwhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuqqoxyu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ysiyeaft.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bsxnypjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xwwsrlnu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ggkxlqcs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fowdjnsh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qfrstoti.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2iulgvycj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ctujxtkl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gasxtnbs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zcmudlkc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2efilaqro.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bhfqrbyd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lhgcwogn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mknentac.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xkklzqbw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ngblipas.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dwzlseij.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wuybrkhs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmcqawjc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cfkitwru.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhimvcju.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cdpcesjf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2txubwodv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2umnhqvss.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cflgumqs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhaiomuv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pdigxbwl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2njlfxooc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2brwsjugb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wmopgqvv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nemoaeyh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2begeedrc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjqxwi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2lsszojef.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lmxypyxe.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjddwqpd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xfifowel.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hoipmqds.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2eopmacbs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kwhitxkg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rakhkawi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2urxqufqg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xbnszyap.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wztvzpfl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jionmyjv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xynusfki.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dcoqzvzl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ajgizhul.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gemzogeb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iewotqyx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bjagkzlx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2znrhqyti.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ilczwwzx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gesathym.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cmqncjpo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2fzgxhooa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ajplatow.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nnjdoltr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gerjigln.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xweramip.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qyrdilwh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rldzrhzf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qmkbdyxf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sovfsqjm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2swouyhtm.html


<!-- 参考信息 -->