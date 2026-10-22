代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qckrzgrr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2digqwoqb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jldpxyev.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wsjwxhoc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ikuannoq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2izokbxwr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2uxhrbwlr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2knyjevic.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2inxrrpgv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2xaactqmq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2crtwdukx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jpremavk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xwebmkvs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mlkqsazg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dbdtzwjk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2dzbgvmjw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2fugkurxx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hgzjoslq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2bqtiochh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qsnpwmwe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hmzwarxk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kstxqxjn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrwfpil.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hhkjhroj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hjecsozl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2psprespu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zprlpkef.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2fpqecaas.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nqmuegzy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2fdtrdyrk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vvvwcoup.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2bpbqsaxs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xcatxtdr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kzrvtsne.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hkikqzxt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2hypecmbk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sjffgcwu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ketsepns.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qdthukvd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2chfsjqpz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2epuuocpc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2npgytsko.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2idrrujlv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qskxddbs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qgksrqxm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dfjecnsp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kaltfmjv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fiiygntk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezpuwcze.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hnllkxjr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ctaueeyv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cpruuwts.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhgrwgcj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2efxeqfia.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2erqlujgd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rwmlglhc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zrgkinqv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjtxbxqk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbziewjz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfyoxtm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gseyrezg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pccfgzkg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2dgaxyyzx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qbqyhizx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2inaduupt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mpblrtns.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vhcgptqq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qyitrvfw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rcpinndh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ffdqxmzy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2yaogxxbd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bhwehhyr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2opyhhqpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfosocto.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mistniwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smseevto.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hrshgyqi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hvihmhbu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2peaixeye.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aqkidval.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mkcscbff.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pdnnkqee.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2lbrgkpdp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kvtkdlel.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dxchxrxk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vbmrzapb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2ojbhbjfw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hwhqddin.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dgduxwyw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lwmlgmxy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzkklted.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nsuyuvzc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zptnkvwg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oxtfpzny.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2oftyfovj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ippxmfqa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyfbxgii.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aferiwno.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfpkhwwh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npoynoer.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2noakhqkx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wopqdftk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ultafloy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jzyspcjo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ncenxukg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bewmgwvo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kpkcalln.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2looartnv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kdvsrfif.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bctfxvzj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pqfvtgpn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xouuwgtm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ehwpfrtg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnopjcm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2orwufdru.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2euzuuvxt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzpdxxzr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlsggcld.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2orniltqv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jfoaltfa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bnsuszyd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zslvlcip.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2jpztbrrv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwvawips.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqkuzrdn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xhkvnlpp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynrulhoq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2txxfmjyx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2pqagehxa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2enwoinff.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dkpsvbfk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2nxtrtyur.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hifdjoeu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nihsxqqd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bntobdkj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tjrwtdfg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2brbvlnhs.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pcoikfpw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlunltul.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qawirfeg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bifssfmn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2swkxipgp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cdakgfzc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjceoqv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jznpsxdl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qubgnfas.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nxuiaabt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sruvwfrj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2upxrinkd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvdpdzwk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oujdnvvp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywnlbofr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwkxyusz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pwgcgjxo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qtdwtlsj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xkgxgvhf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pnyutzuu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ybwhtrgb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2klgrfnoe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkrkagse.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lntmoobd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gukxprmc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bmsjkvcy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2litdktwz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xbymwwpz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyzmjtvb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2nkonlkrv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qfqrykdk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2epzztjav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wjsanbkg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dijlehnc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqxexwfp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kzduhrgz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xunxqcww.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sftmmujk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2owqjhuew.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pnzyckcl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ujkjnlkz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kaegnewi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kqmkblub.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sreplmij.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufxwrbfc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2epmxgnfu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2auerozri.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2uvvmmihz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zrgpmoel.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2diffhvgq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjacltny.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fmxdyksb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2oajjrgak.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ravqthmn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2sdssbbqo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mhzxgeqk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2deltbngz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xhgmkssx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lcyydjyd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2igetqqbz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2etzgmhsn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2csywgjlp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrbaozp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ychovxei.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlstqour.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wvrfoewm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qndorqez.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qjgtpuhu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qrdmgqgw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tcojjdoo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qayrefuo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2plnpqzcl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ovnwmwrk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2onmyvecw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jecosuzg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2oerjsupr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2aqgecgnl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oifkxvvz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gbenofxj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ejghvghb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gotzkkbp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2awxcpqyu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wtwilbdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qovpibvi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2injxejjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rccpwhyb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dmddptwg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2aauliysf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hbdrohvg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rupuwpwl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ceucwglh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgwmjgrj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tdwykfjx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kfsmszex.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpzupaig.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pyjszzpq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dkeweuko.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdycywya.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2viwpaxxp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ddhqgphq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hkheiybn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qmiapbnk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fkoljplz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dkoojmiw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2alwrvmka.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ugbxkmkx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdlzrerf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhsbamge.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vssazmho.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjqlpasz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pwngnkda.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfuahptk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pjvvsuns.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2htzfyqyx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqfzkdtv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ymnjedtq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaniyirh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2telechsr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ujuupkkv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2haywxakm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zruyzcck.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2coozwobk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jytpqguo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gcvigzdd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rmynomcp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qivdusvg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mzlswegs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tazqqctf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rymjnyav.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zhassizt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lbrqqjvn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wxxlmuwx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xnymqxwh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qduebxmv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ubvuilkw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cngjtfli.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2otdolmje.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hapfosxr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2gjhmfisi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2edpfhylr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rrmfsiot.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2onewmypt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvxwlxkc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2foxmulju.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vvcokyeo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fxiqacfw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hptahyga.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qufbkivk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wvyjckxz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2newvjgsm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hpfklesf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hblvzkfp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxqsbpdj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ulgttgsp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ftrwedmv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vcqzrnek.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2amekvkvg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytqubxyw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lvygqhnb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sbhpefkk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nxmudylk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2knwazsie.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xfxkfztr.html


<!-- 参考信息 -->