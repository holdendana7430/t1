代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nlgtlrlp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tosiyjci.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ateoaxhx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3pwzigmxf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3cegmkzue.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lhdqiucf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3cldxhdgt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ftzrcpco.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tcvhsfef.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mnovbvyl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tqqjravw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ackkjyex.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3czkntthk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mnfaxstu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sotnendv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fjrcstfb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cbnbyign.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cshnnlut.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3cgtgysgr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3kkdgxkhn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oxldblbj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3wlhtykax.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tndkvfbs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ndmtnmlp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hgchcppt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cfdccmrm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nedyxrqd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3efxzmkgn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pnlstguj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vnzpbjnw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vzbuafvt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3davchfub.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yzabhohq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dyxmoupt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3voozjqnx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3uoxjqemj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3uhguwbwm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hdytvhbf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ymkyjjyy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fntogjvp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nprqmhiz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tpgywmxb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pkahppjz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ralcyesq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3sihuwmgh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfywosts.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3slcsqvnj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3irsjykjn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbbotxkk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnfyrymg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vckxozyo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ioxgwyaw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gdddllyy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nidupccf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpykobd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vbfspovq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ojaqszqg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zhddozji.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fntkdpvf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qdccdqjl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ajrjqyvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkjifcid.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qmghhtik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgswdylc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hgwsgboc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rwnmbhmp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3cnbnwdav.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3frswspol.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3swvthbzm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kmymgoba.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lrxluuxh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rleoewek.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vhvxpftg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xofxihny.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jztyhkkw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwctpmlw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3prgdatgp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rhepxjqr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3niyanaaw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xltojgoo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gkqqohma.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cgzjzuwt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3rjgykuqa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3nhjminhe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rapaxgtp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfkrtuum.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qnliwldm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3royirgzl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rxwldlij.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ibogdghu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3raamnxxe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iubttduw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jurmenua.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3rnfcqwxu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ibhtbnlo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dtzfcutt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfagtzu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mexstdgv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3letakpgd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nlpeirmu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hxxrvrcn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pevwwytd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgaekhca.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tutdvvet.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeqvpebt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nmcrxpkx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lmofgehw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jjvuutaj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjldvrkt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3zxtbboho.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rnpvgprd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wspptkzw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqeglpld.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lguzmben.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sebwqovy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3minpngqv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hhcwshcl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3denvhhsc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jtledlfk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jehotcxe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3myecwiwg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oszjeits.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gpiukuec.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zmrrnyti.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dbqvexpo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jpbxnbyf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ygjmgmgx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3euapnuwg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3maazbnve.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lxzljbtl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3inpqvdvo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tjbyorbc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hykipqyo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bvyzrfnh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lvgbeihj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3occntzfd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3nvbmutue.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3flumofuc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ogxcyawt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxexpzcu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ohxkdepp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyyjpitc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3usjyodaj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yprenfaa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikgxmfxd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3uckundhv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3eggkxrwz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mmkoyrim.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zxjjwjfd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3djkqcxek.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kwsyxxbs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3naqttirw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jdwxawrk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdnlouzr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wyounqdu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nanpnjab.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jxviwise.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tihgydxa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gggxdhpf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3wiyaqkoq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3grrzivdz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zervtpkd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ayrdsfeq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hblrsmfr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zlfdpvuc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3cizqtpng.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3voorvsux.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pcbvtltj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kzxfxdbu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3louzgflu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cqnkpual.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mgfizljt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pvvqykzv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3alnwdaov.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ywnkvykl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3aobdmhha.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlllyyjm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3abhldtxs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gvsgwvpe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xhmbrtxu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3exbvfdcd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rxzuwccy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dkqkjpvv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xeydgjep.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3skpcqvto.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3updptjgl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtsdyiha.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmtienwf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ubrfyyst.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpyfewqo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gkxgsado.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ybdqnnbt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jrzdzyxp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fodpygcf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ahjdhziu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3moprdzyz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ccclziuq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dsdxpviv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aedjxakk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3srcjlhqb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dibjihwy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dotlktij.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qyzcgycw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bfbusdsm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3neinkxuu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xflciaqo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3khgyiwmb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3baornpms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkxvflig.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3yjtbdpyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymvrkimh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3migcvmom.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hmjswwfd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnrfhhrj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wyhsmbsn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ielaihql.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdcpmycy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lgudcies.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfbrarel.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3njbaxgsq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ilayfdyo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ojvvbjxf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umltufig.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qyhufova.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtsieeqz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jnqjcuod.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vaviqmhv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tlnkxcet.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mutqiddk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uoabcqcf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrngbuy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dldkdcbz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsveldyo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kgqxhrdv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yigkiuqv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhydnwc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ebqlxrly.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3iomznqnw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3szwgrnyq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3leoejugh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzbyznjp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xrttjrej.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3viqkxpni.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vsnrploi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvnpjoav.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dooezqak.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sxqkaqad.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hweuphgz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qkpdnyez.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vzzlhafg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3erumauyv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ghprlpiw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zaqmigvq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kjcuohfg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cersetku.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hfeqrniy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vypaoxby.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gkxfocpc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wuxiqmjw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xwvmvxis.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vxidkzzr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rfxjflzj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gtdmiwkb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gyllgjzo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3guqzukbw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gfrivulm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xrrcilrq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zamamsue.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ttxdouqs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cxnqzmzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jgqagjvl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3mdulqffi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dbtfscam.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dfnacfto.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zokkqyrn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xqufjfxl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xherrmdn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqslsaos.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3znzmqupy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kefunlgr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3anwpnfna.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3agqiqnuo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jipdwrwi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3llqdezri.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cezuvgwx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdlfkwvy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kanljhur.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3guxnaihp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ownworqm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fqobvtqx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rwwiroma.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3satbtcte.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zuaxltmi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kwaqhtbl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3unbfeczz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3brltrkyh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3shvryemj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rkivjekn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hnkfkxbr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gnwqpnkx.html


<!-- 参考信息 -->