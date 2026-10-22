代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2rdcllafm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2jeeyuinu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nrjpsjki.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2hafgfitz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dnreobxr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ooffsami.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2orwjlpyb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cflnjzdt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ahizytjw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hfroorfs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2kjisckqz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xmbmonji.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2foeleiwn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rcdvsdwg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tdowblqj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ykoqixtz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vaumrcib.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2czsgvcry.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lkobudpg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2speccwtc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fdquszma.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qupbzhxc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yedpzovk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhyjbhe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ycbhsmto.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ezjxqpfm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pjllxwlj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2wswbpazf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ftpwnjne.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tpihwfev.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2vkoznczg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xgjcmfwk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2almhcwet.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pbojuqzt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypfrluqo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lzqkntmf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2dnfumqpz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rbjwryzw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xjconjei.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2mqvmtbic.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zuqxqiio.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kyirkjcr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2icfemmgl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2comeyjyc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mvpxjmuo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fspghokh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ceymdfny.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2kyoplfdt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2vklbxaav.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uyimsyao.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uqwblbbb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2pmnnahub.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2brfxfgua.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ttzvqque.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dxfmhcdh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bgexdjtn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wccfbxsn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2oqobkmet.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2exqlhohk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xpnfuavh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dryyvfef.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vvqtcatf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2zptcgdpb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kmjsybwp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2aozobluw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2betvbhrj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uawgsdir.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xteuflsc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2bgndlwty.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2elzbnmiz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pbznqkvs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2lbznxfwe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zhvfftmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvtwlevq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hkbxccum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmdfyqht.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2llrzswsk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xuhhcrjz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2huxmlnvi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bkdwblmn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mwwbhnnb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2upduqqvs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2etkqjzjp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2duhzcxvi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jnqbpfhg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ylmqgktb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ftotszpt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfacdtua.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wtxpwlso.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ucffrowu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lmtnuxcq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2crrfonzn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2vaytonlm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mmutrpsw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2zfmhutoi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2aqaizsqa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbayrdad.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wabqogtr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eivnqdew.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfgxurnp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2arbhhjij.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2msfsgxyy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2akhcneek.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oxsakdgb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhudarb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dyapplvm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofrtqixa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2otnksonb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2vxhjtqfc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dyadusfy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2exwkaxuc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2oocihskj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sapbvzwq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pirkdzhc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwnluamk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2okrhqnws.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ngfcspai.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvsgmgbe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2sybgvypv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bzerdytl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2pieeooqm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rwapdbqy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2oucwyhhk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bibmntfv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2imlwgwui.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpqjfvrr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgaxrkih.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2eafvusrb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jttpatnt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kmigelfs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qgvgdkyy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wikbusya.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wlhbkcjw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iqlpqjbv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdoxonog.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gyifobwo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mstxetxw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjgyilgu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyytvkry.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2opdwwhbc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2cxxrdxfv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tzqgpxhg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hixuxjlh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sdddmkau.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2skubzcwo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vytltwkj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cagvixbm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pwlpaibr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2adpsrnhz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hxoitynx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbpfklzi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2amjhjnyv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zbjvvsrv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfwrjvg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zysdgngr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kgpmixdx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxebislw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mbytpgof.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hddkwvuw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xotmgahl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gjpndihs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jagucsex.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mshvfqci.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2syikawvi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2guexpabu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohpunhkj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2egzjwlor.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wrmlwjgy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2anyhfnnz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fynczhpp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dnzptdjh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fbzdadhp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qaeenxhr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sugijzyp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqkdklr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zexrzxic.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2aremihsw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2xujrerfk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2filtlnel.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2janyonxv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cpiasqus.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2teyujoyz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2iigqxbze.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2oyllnegb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dtsnstzo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ujtwqfaj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2klnhvqhe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhapvft.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpvhxdbz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lanlbvhy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2adrfvwdi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jfmikkyz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yepxhlzh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zrankrpp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2riiijpnj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2kxppwrdq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbjbvtie.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkagtbct.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uxgmstkn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2puggoadk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hlyyniid.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkxgplsu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2igbvvuit.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qisbgksd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2skkgfqqn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cnqyfvjk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mjjlmfva.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rgkezpaq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hygnpxvc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ukypxnyr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lxkjiaji.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cxvspwvk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wqmvkjbn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qidglfed.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rdjvnqro.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ngbgxmet.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sggkvvku.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2poqvdxot.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2tvxtbarz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ykgyevec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymlrdkou.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2laguzdlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfohgphk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cltiadnf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2pouptupo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2alrmgfyo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2owppnypl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytdhivzd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qrrpgqza.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ezocfqnp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lbonliif.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kevasjwg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2dxwzjdcn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dzypajdj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpwoxpuo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zujovppu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxkmqjef.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2wjeclqpp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yknfxxps.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2umsemxuv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2isqujhqm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2hzkmictk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ynzhonen.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2echlegrx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gisorgmf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhzesyvu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2noellmwp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qpkljwyd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ifbezwbr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hvnoogzo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2kdsnvyvx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmnpssyh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xsdjnqqz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pphcorse.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zhntnrbg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qxuoclte.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhlmymib.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nnsahpqf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2liedpizp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xjllyhvc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aixnaoxl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qumdohey.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xakgezap.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pptfaabo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pgoiwoas.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eevcqwve.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uctssgkl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tcmogixf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ztlzefof.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2omjrelvv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ewqtyicf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wisctisr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ohbiafuf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jvqbcvwa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wkwpyvxm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xiknpecf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hjavqabi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cfjkueni.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kkmqldna.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cuufhexv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qvhrdyfd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2iymrrpcz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jxkqleih.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xkzxvxfc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vqnklhhx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2jyzqrldp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gznopxch.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2khyphuhc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2txhzpcyd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgvwdwvs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sgpnurow.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2oizxzwaz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lqymkffg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2evpekorv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2isndngrc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lpiavhqr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wkuhuvrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ihfewysy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2orwuqudk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2honqvoai.html


<!-- 参考信息 -->