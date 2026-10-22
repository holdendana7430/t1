代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2nfbomqya.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mxvcyiyv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zntzugiu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rxhhexer.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2amczihhz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vkupugda.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2kiapkcju.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gfpekpnr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2etfyllin.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vhvblscj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2onalhgrf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2cubnldjv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2coxmdxyv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xbrlcvtc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bqarexdp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ceonqxch.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2xulduicn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eayzzahs.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qxrtchan.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsticihq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cwagfkjn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pafzdcbj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ojbjazxm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jtiqvbip.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tetndavf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2felcxtua.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gycjrjsu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2kmarjjci.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2menyvfpa.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ekroyati.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ugfiyodg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2fixvvtdh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2euvqwfvz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2keezdqwq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pdpkjygp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2peytdbpn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2srvpvtax.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aqrwrhvw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wjffefsc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mcyqaetj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2emknqqic.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2eiqeqkkt.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2yappoknk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2wieclrov.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wimfacib.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cugdbajb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zhrtfama.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wvsvdhje.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmhnhsll.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ubslbsbe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2icocenek.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wcjgwrnc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2kjozvgnz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dnghcbaf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vatibjfn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptailzmj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2bjomxhtj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jyrwmmtj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2bvugihld.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vebioscm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ysgpnjsg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2sxkoarmh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjaquhp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mwbgdxku.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2oikpyufq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ukmhhunj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pxpqebra.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wjbtomlz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kpphrctn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpdbyxoe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2djavffdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzlcquij.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2oubqddll.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dcrwgazf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mdvgqdnj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wdohxtmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2junmxsve.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ybeqktil.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gnopvvxg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fzqgejmr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nciqfbco.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ypmizise.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2sjrpebcc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouknogch.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xqgpuwll.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wvdiubbw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tlceqrcc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ajwpshbx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2llaqrfcw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ttpptzuw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kwtwftjk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fowtpqmd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kliakawg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uyuqddnc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cdaqbfaf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oahmumwx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mrnfdocu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2goexfeat.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2osjwoxet.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ophjkajh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vswtnwqz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2neghpixj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ykvsuvje.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekwqburu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jiqhhncb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nlxuphff.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ysmnkcci.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mncupnre.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kyytzopn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2sbupojcs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jefkqowc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nowgngql.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mwmpuxyb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybhdhjwq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bhlkgidi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bjujslcw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxvtfbba.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2revgmswq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mslqjprj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uzwcggri.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mslbbidy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gbdruhye.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyzngff.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kxoiwafi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bqiaboyq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjoyzufj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xgagjtwa.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2valqjwxo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tjeebpyg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nuwyvfod.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eucxdzzj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nzbtnaps.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ryfbzpym.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ckegpbna.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxqxlvar.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2razwetas.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xwbtoecl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qkegavpl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gwxrrcwd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ytdruwbo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zmextjrx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ivahclqj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2eoohsfau.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2naknbnuy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2durzmdtc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2okhfhbhb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cpsawtyo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kypxnyli.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sfxaanhd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dogbzaev.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gqlvungo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2cnvdlxcs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjhdeuhr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2caimobso.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ybfisecz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tpdsrcdb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2icykwrwh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2snjvzyzl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2juphglgw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xilprzjq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mxmsprar.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dfpsjvvp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2kbkowsca.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lpbiiayw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kypxasyt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bhjeejxp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bpsqwocf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2coggmqmc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rjjivsav.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rwwiuuwk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mjbncmtt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vyydvvgf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2eqoddmvm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bskoltdk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gpewlifu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tdrjpzfz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jwgydtox.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vivbrdje.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fthvikvr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2oarqafzv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bkqxoktr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xgmwsovb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehgaoqgr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wfhactji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qramuhvg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ntbwethq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bvpxacyt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2sqspnero.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xxctmdye.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sjvtbntt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2prscsohj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2bqlymygs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2byofpepp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lbruhyvy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2omobzwhd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyordqha.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryusjjtp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2shdyyacj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wxxbfyvj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kcnfigoc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2uxflfxzh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ztcyqybj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oniaxdlh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cvzbafyq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2awyibann.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ocgeshln.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ljrdfzyo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nqeormoh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nvbrqmwo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xauzzebz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pqmpzaxh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rvaqztbb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lsmkgwci.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jnlajatu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mdkaxgka.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ejrvqnxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjvokzke.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2sylpviro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xeapjzyu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkgiozic.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2muvfigrq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzepzjpk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oudrdyky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2igzsajde.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sauhsoxm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xvhagbar.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcsjaoeo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kodqrbys.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2lzzwsbob.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bnszbepi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqmlbbqj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2riunjmtu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thdkjfhv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2bdxcnidz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rdxwwevm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ngezotpg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2illqgrqy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmycbdqf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2drduadeg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2liltnobw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2swngsdbb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kspmdfhb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2diwluyqq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mbkxilft.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ebbyjgvo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vuipkzvt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mnnianax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2adeeuwqj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jistkvmo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrwljmky.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ohjnpseq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tgxoplco.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kqtoubjx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sgjateji.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ochiecnk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kderhifj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ugzegsaz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2srqxpwep.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cwzughbr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ypltdcbq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2omtefdwt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jgexvwlw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xpwtfqvz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2wdbhpzry.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ctpgcgya.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fihkywvb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ivbnnwyk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2slmpsoml.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hhkteydy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xyxmxuhj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2niytkuay.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2smzvakex.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dlynjogi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xtcmeleh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zjordexc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rwryxjss.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cgjtbzcd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkjasks.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vpdwpkyq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xuwspetk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2agozsfqt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xdtvvxuy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2tatishqm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2korucoke.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vyyfghed.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fakjlymf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pcautehv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mpkkecnl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2drsseqhk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fjopvypq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eekkvxqw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tgsxkcxn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eolhmgyj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mihbbgvd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ysrbuuyv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cgvqbtig.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dvvjfvho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yxnspvrs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eendfncl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hmesidzk.html


<!-- 参考信息 -->