代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2tctzqdgp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2abjofujj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xyyjsgwi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jvhnfump.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2djggirck.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2amiqqufa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zeklcgfl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2gnrelsuo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2txpstsxk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qczbuhuq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2omfnikxk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2pyikaxen.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kswkdqcv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yukipamv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2tnlahkmz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ljmnnjyx.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sugfncmc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2erjmiiwr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hdepogit.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2eshrpkwu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2iyxphtpx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jwgfrfxp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2otxeewtn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gsgnupcn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wfrkwztx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2dmnwmysf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rflwofeo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2flxpefgd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2xkyrbyfb.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vnwfvsyp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dthvmjom.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2whgyqhvb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zfsptwff.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qtrzgemc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hloyiqua.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2aohjvbcf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zecxpsyx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qxxldgdh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qfigrxri.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2eaehjjqo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qzjvadik.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ntbcnjca.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2sstithvg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2miaiukum.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2skdkxrlp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2edoymyvm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qxebelsy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2qrdjpuql.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gpyibrlq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fbwaibxx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tplewzpd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnhginhu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2btxesmsl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2eimflffy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qdluwfre.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ruetoybk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2weotnhfk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2obiaecth.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2puxbshtn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ciukkfnh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qmtsnqck.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tuesfomh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tqjjgqws.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qxtxoohz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2opipunge.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2qlweykoh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ghpfdxuj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qvtwgxid.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oidftgxy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgcwznup.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2oynslwks.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2djkkkojw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ulnjijof.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2oqmvwjbp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xolegbgv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2gcejxmff.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qqwlkpyu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yrgvwnhc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ymrmsvvi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vxshaiba.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nnazaxkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmacxcws.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fkgxofwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdzhazdw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qmdncycx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bkjpzztp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhfhllua.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ktgivcyo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vzumccqr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2epkxrrzb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2zhswbutg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ufldfnrk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yespmuvc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2grtbkkek.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2jaicsphc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bnnmvkpk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2naedkayu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mapvetff.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2esybsbir.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ayacqkri.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wqlddgqb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rgdyhzfd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hlqhkkls.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2niryvsha.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqeemnfp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmjhiah.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzpllrwi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tlxfbiaw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ygqkwmxh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sybejtzl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ppvluprv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hbnuccgz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ukjaypxn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jubpgkrn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxumpwu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmzudxal.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zzkohizr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrgifgra.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2soejlpix.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjxplhv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ufthxkmq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kbuprmkh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2akeevxgn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wqtryrjw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ybnmlzjx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2nkyfhuwo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2royjpcnt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fghftyxv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ludbryrc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2brngjeeu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fdhoagem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mstypsmb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2flnduuha.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnucuccg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gztdkpsr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2wdukvxrx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nxksauza.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fesivhnc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tmwggwwo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rhigpagz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwvstslp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hlcszgrx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2migeobsu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdqwoqak.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2olhibdie.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2aoemncqq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwscljtj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2tlgyjdws.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2qwvwnnwe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wntsbylx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vamqtnbi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tkuxrchw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wwwkwhbb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ngtcljwt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2raewnsmw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2unpdmchf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2nsislkgi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ucbdxqhb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfvoynpl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpbkachf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylrcemxl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxikglmh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2luumplqx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gtyqjyvf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nsfwwrwl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2souxnekk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2oznuwies.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2odgqocip.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2daidfhgu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uoohbajm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jycejtfm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbpfvks.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ahxtnrin.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qakuirjt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ibwwdhwi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lrrzrnxh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sebbcqlb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2scxcffpr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eeapfcxx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mzezmxja.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ewhdmplw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vyzppafx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gmlspeut.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oogacelm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cbohqjfm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wezdyaan.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sthxezcl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxysfita.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ncmibhqd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fnrudbzk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kpqvjawl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2qjquphwz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zunpjoxv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2khbbypuw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kaphemwi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlhgtdl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dceqrnyv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gqgdliry.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xyidezrk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2izkjmbnd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dcixnjws.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pchflnmu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bzxnxxhg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gywfimfl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zpjfeuhr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhcnpdi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2orzfhxcx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ugkgoosc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qzikbaec.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hedlpizu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pxhnotap.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2atlutizg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zhkpbleh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rlfinkvt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lqzsntfe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fuxtucwz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hfeabnkp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzbzdxgk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wamlxxgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vrhfgras.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dwlmghuc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnvdykyk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qkxpkody.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uogtpjci.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2syxyfune.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pzkvpyby.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ziqityac.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ejlehkbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxuwagnd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mhxvptse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpblfbey.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ehkpdnzu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qrgkgqrq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oyjlcbha.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qbxmdyje.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pbeilape.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cilutdfk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jkicxcsm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2flxymxwr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ptjqpyzv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzakzxii.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hfqexzif.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbeileb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2waufzvpo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irullixz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rjyceodd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ooasrbjd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2thckgwal.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gbwijpzr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2yzgrlfys.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jkxfkehz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bfebueyl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaqwrkxz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2huksasyb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbfgleex.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qznhhmlg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fybinbwe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jyhwsirr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2irsqqgwt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2thdgbmsd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mtsvdxsb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsbcohjy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ctiulbyo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kcprqvqe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2eifakesr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhusqqmp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hpkmshkp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rnlepdke.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rkppljev.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tyuguwmf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cbeaefat.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ifopuldv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ieeaxspv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dvmydahd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zamyqyes.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2btoxqrvs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jpblvbim.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kmvojrtj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ygakcwmq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wkgfvyio.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfwtueqm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2unfwjrlt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2juxzdtmw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jvwdsgbg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yqanyvjy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cjoccpyx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gomjbfmp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mzqoapjr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2okirmxkz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uujwrdlf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nqigimtc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mlkoaxfn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2egivpewg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tbqqsynw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qkmhczxf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zwrhzghx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nobykrtv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdlqjjfj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryfvbolb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dlyrasgq.html


<!-- 参考信息 -->