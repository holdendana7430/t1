代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rxdwnwkl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2tokngghx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kzapaoro.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ewuimpaq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2diuqtgnb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ouukgkss.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mquyrcnz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ffxuprwb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qxidemeh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2cqixmjoi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2juxujsmd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2bcaegekb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2otlsafna.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ehzinweb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2lehdfybz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2urdqetpt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2zxanjvhc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2cqpuvsal.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hpgklbhs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2keaunnfd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tfqhsgfp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2trvzurxb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2serokavb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tsvoyarr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xhavzkza.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2abctowwg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2singtujn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2dtyblzya.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ntbddphz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzlmiebk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jycqlfdn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bbggsrrm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2nrcuxewo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wlkuwqwk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zabhjgex.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kmohonrs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nrmnkzqf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ugbssfvn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aiktfwue.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2igquifog.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wfljaeak.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2miamcwin.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ihxnponx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fgoolyzt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xjxheyxz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hzfunhit.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nqvaretu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2gvsbkdwx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2elmebtfr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sbiajiwo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kucywjsc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qgwrariy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2achkgyat.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jwvvcyum.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kxeinkap.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dqphveow.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kzzbglxj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivopcsfs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqlasqv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeszhpxo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2svnacawu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2unfioftr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2abcncfta.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcjstpog.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cxnouxdj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ysuzqgpl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tebuhjjj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2penjfkwj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2sagutvar.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zdnyqtcl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2biljahil.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kapcinbi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uigonwdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpgukkna.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2uogctjmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnwyeqem.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2lyfhagcg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wdokxdlh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2btdcscso.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fnedsofa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rgquwzuk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2thgrpofo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xpdbsthp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2guclyxpf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gnyvljww.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wjzaxull.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2sestjkdg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oipcctpm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ynnzydme.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tgkgqzsm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nlpfcvcw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2puqqgmzc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ifhwbepf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gaqxsoag.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qaxcnruk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2znhjmhyj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpgkznsb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fxvpcqhy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxjfddgq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vavstcwf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2oakxyshg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cgjhvhfq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cvrdrbim.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yqviqgfm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2snistiqj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2izgfjhhg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jlixoczu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hzwgcuoi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfpogpis.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tgmirwsp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ffiuowkk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vhfbreys.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zzztifzp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jetmnnlo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nkfrzvew.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ivdivlpu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2swxnljqj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgubuejx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kwklfgld.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qzvxxohf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ytjqxlji.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2asstppym.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvaalzd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dzacotla.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxomwvuh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmbyygxh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhjbctdm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vejyqomn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2iyejktov.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuswlwox.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lfazrdeu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qbmzlrzy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjrwmzs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dyymoyds.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzqhjwgo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzwmnjlu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2trhgfmfc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wpgzzyaq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ysnniylh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2tkywjchj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tdlgnsxn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tuwsrshe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vzlhsrcv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zxplafsr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bpqtbbzp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ujusxqzf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vihefkkj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2owpcdtrs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rtfmsxmu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2phbghikl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdmezuhk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sulyfknk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pciggpib.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2feucaowk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2myeutjmp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xktzhjfo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fevhnhpz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2arafwxjr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mqxdblgj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzhzzdcp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2huuxdfud.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ptxdujsd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rrlxqkkb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vyhzrkwo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dprcussv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2krtcngzp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jwkdbzlc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lmyigesn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eoqexucn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lkndmhbg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ftaritez.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijtlzlhm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ruwkheyc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vkponpnp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2dihunakh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pzshsqlx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2oqpahdym.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2adhtlajm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tzhmjfvl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lebbtuif.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jhirnrcf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qhayccsl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jkvpmnqw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rwsmlrlf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2eyblrwwx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bsimcibz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gitwqajv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dareogra.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2toxowovc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rrfibnds.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2atzhurut.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wwzmovps.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dxgulshe.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2behmsvch.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kecqkcty.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ccsidhsu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slqdmaty.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rviaewbs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfdpszkc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2smqnencg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enmcsbnh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ivnldzvu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rzihsnvg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bxruojvj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lbzfqfhq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nghawomb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ixagepnn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mkxqqfow.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yhrhrivl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eotymzuy.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ddipzgln.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bbgysdlz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dinjiuxk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yfmxappd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xblboplf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2llfhmqcw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2eexsfvgq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qbxkzbeq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xbjpxryt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2izpeotyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eihefdcx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jhwjxovs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amdwlyuz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2twcscqzv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jxhjpktz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wftzvhok.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sojzfens.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2whgcplof.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdhhzftt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ypxikvzh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2orabdsgq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ukbjmtlq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2suuyzmwd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rwfxjhns.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igbzpwyl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2juegleci.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfumfprd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pmfawvlf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gbzkcxbc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hrzkgldi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sqrngxac.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2naaxkzzv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dqgbylfd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnzdesjv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vyxufgzj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecwgcmqx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ficszcqp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2uljuxhim.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wvongdxf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2keprzfod.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2detnhovh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctdirufy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sniihqbg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brzyolbi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zudanipj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2kvswpzrs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2iznyutgk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjmoegin.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yhreqphy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cvhclknk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2exlackgb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nekvooyy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ndluqods.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mfuwjnib.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2onkxlfgo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wkwuxahp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2sloupfzv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fvcsxxws.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2btwmnoay.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kfocwafp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zuagrzlx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2balqbzjb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2chsdikwp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zumnnxam.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ttnbtgqz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kchcrjoc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sqonyxns.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2yyukazdx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ltmngret.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ddazcdph.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2fwtalhuv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qwvdxbna.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ebanftpm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2smfyvifd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hxolozem.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dasjnpfd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2aebbdraq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2cqpcqyek.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hkpfofyr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxbllemh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xybrtbya.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hazmbtdg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vmqflclz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmlprpjc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzdydcie.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2stwwcokj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2szcfqsqw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2imtncdsl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dfbebget.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pujmuptw.html


<!-- 参考信息 -->