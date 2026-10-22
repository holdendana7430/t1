代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nheezpcn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2nerkmmpn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xtaboebk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2robcbziu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tgylomvw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lighftnk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2shbrzryd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2clolkvss.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rphokesy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xowpiubu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xymjmrqz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2legerbmq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2edcroxfo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2cymhimvz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2zsvnrehk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xqdfgctj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qkbwtvdj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ipyphvpa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2slrkacdw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gbgakxpy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iqukihen.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mndmwmja.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nyuwgrjj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2phdsejkh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dwvvjemx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zqlzyhhl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2szsuytcu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ygplveqf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qlsakpdm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jaoqfqzo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2kftrlqin.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vvsknict.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2huivhzoh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hwvpqbmk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jmrcgbbb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2sooaxocc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hldagfyt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2voyyyhyh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ukvpodlq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wkqswwmz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2osrwqnot.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wiarfytl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fblbhilt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zfmuydvz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2inwwxqmj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wxtuwnsc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kjbujhkb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mdvpnkma.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tmdswzkg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ntgtqfky.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kueaeydr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2efpqgiwb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lllpdych.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2duaoeefe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pdfhgrhk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qliuukjt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bmneactq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbortopp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ydaaqpcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcrzkkxp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2plqswjud.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ecscinrg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrolfaxt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rhvjkabb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vcdlkbjg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cillqxfj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2iobgxzfv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mtnrcscu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jldjwfsk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2snqwqjec.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ktpmutzk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lytfqyap.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sysftbus.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tkpvopuf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ifrxvsjx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2tivikdnm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kvpemcjt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dzovhnsj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ejytvrcy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kfptwddj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ojkefcca.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qcbpkpiy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqzfwjd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2saxkklxj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sucyfpao.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jwgaowfa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2txhaiups.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbhydkgo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zkixahmg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zwmwjkbo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2paapqytl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hdhwhqpo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkygelyq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fnenmkvo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2axhwbkdp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jojutffp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2klaxapxd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2rnszytoa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dkunwldw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ntkdvmtm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jltdpkyd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vqiochuv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qmgvmjnq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dxjgyyqo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2okweaeao.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vfdumzcv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2psedliwg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmgvwmv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vcwqemnd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugyrbkeq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fusuaisu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqdqmsk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zhxjjozc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hahzzpif.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjfgdmrg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pieetorq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sutirngg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ajgnsucz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2klugfitn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ivvqgvne.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2apruzgio.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvpnwmce.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnunytsj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pfgdlmeh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xvgwchzv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mdruehjj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vpzwweyp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kjnxitfy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qjmzepno.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bzqoykyb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nuzhznag.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aktacmsl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nalkhlvg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hxjvmsxo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvpmyqfv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lirfsnwl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ekiffivw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnqhqafy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jpxtbxyn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yjzbvlsl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nduedohh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ujdkdoca.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ounihlwm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opifhztd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fvterxvo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2iitugnbr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2kqwcqvfm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmpyleb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2eqlikqtg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ruxsnktr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dpkalkaz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pqccilnz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nhovljqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wreogoms.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tldignyc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bfjyisza.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hfemjtgu.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tljolbmu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qfbczijt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zaiprsbe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ojgtxnvl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2dmqjuxqp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvcfafj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tmhlyqdn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yvutfmjj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gdmbyfjj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2wvznomjb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bsbtwjzv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mkriofbq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qyfdtgbu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bnfauipz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qashfksy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbrubxj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2focoqriz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zkbqgsld.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vkexjjbc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vmmvueqq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2eogtrbmp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nftqhhlj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lszathbx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2poosjiqu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kcgbwbxc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jydlpwal.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hrklovjn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzicrxoc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2catwtxrj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wwahqyth.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2isppbpnq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wgzubclq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hhgmxpry.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hqwikmdp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2abgkcbzd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uypxvpih.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hnmmvmlj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vhykkjot.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ubjedjfx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2eokguzli.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2irigdkss.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ubbnsqlt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2piafxgvk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eilyyfcn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkqmldk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fpqhxajh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lubdtahq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgpeeuzl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2givpkdkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnyrkore.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rakhdmhb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vpmlwbkx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dsnkffts.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2edjeymju.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aqptohcl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2msjgkrva.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ggrsnotz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcpkmjev.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2axsvniye.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cggqzlcr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gmhtssgd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucvlryvi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqqzdxzb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgbnpknd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ehaxxlkt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2rhafmiwb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yoqxkauq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zdkjpxiu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2svgcexrt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wsmnqiux.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2eajeaqad.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ptontdpv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oydnstle.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dfrgtvki.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zgtzizww.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zpablaad.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qkwqzvdb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qmoexqkn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zcyusngq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2amehssbw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kuyltvhi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ddmavkwp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wzlnxopr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2aytrxmlr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zefncbcz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjeewst.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2faazskkc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ppvzckos.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lawvypfo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sjizlpzj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2smbwzjaq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vvbxzfie.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ktqnzjko.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ytwscirh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jynunfhr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2iqujrbab.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tmkbcfjh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2eoloucba.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gpkzgfva.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ouvhvqhk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ykadkcpv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pyiqmoae.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ielacurz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mxdgxlwd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ngzongpy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2exdrhgxa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vfpsuqfs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rrvyhdyy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2hxkihwhm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2njshwbok.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2iibfhumu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2eshvucdk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2orincupc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gdisvfud.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2aucssalc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2lgjrjyjo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofldmevi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nvqirhpf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xoscntyg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2jprmiiwy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rskntbwv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fmktctde.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ykjznvpc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zkbdoxls.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwewoesr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zsjwwgwi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yzqyjsjo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxxeknrr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pwpfyzyr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zvztschl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qfnjyrcj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qlimvxga.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bcfqmnaa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ytrcfqja.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2iyebghgl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tfyjwasu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zxqimjyd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rwjhrrac.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xuxlhdgx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ferajubg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2edxeilyv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mfsuxjmg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qfwmstib.html


<!-- 参考信息 -->