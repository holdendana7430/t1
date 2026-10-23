代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pykoqqsd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vqghfutx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3suvepqpf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vljxkjui.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vsaphtut.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3lvcfmfzw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jswazpll.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3imxhmuqd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cqdnskmh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahauemuf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3szgaytxr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mtjtkmqu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3iaqwazkp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nyyjdtfa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3elurdibl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wcremkgt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3quslvhdc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3chpcjfur.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3aoufzyym.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3msbbhvni.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3dkjirvjx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3sunlmmwu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pccmkswt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wccotiiv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3yrbfevyp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bipuwkni.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fjrfgats.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3rtbvmnyo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3aohswnvo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wencaucz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyaitzwg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxnjsov.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3npteuyfh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3etlcxtle.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bglclkci.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kdxojhpu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eyuoaorl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3izyhvymd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jnvalvwg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3sbmvnfrn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ojgvuxka.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nxkwigrk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uilziscc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3skahpcjp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wlxgmain.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yzlkfjwf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xvufwchp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3loynfmwa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qskfdkiz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ceyzwxxk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3txlcpggx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvpekyzm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fudfjbcz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3eyjdknxi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3offxsbcw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3plykesxz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vpuwbqub.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wdwdeptu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jrporogu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lpqzqjxh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkpgancc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3icugsfti.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qsvhfsft.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cjfrdacs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jkomqlbm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3opiyoegr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xvwrwjzk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncecqmed.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3puwbmuis.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3smbgtbgp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fpyuktqy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bmagdwux.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3bsgpospb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3obvnfysb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pgtxrgjf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ncrifxgv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rxdjtvvm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rlcpbaqf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zctyrvwd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3yoptapco.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hdmupobk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbkreefz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bkmvpxdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqjowulr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3htahlywc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3hermethb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sojgguvj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rkxtyrke.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kvitzhrg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xgcrgreg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3phkgrlgu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3slxyowht.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dekfqswb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xxyfipsv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wetmlmvl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooduzgha.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3oomumgzy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aetzmcso.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lzaikiwd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mcfugbwa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kcqkuuxy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yidbgkaj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3dpfpoxuw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pgmhytvr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oauvzkwk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cbenhgke.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wzrudszv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwjorhdb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vcyvmzcq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3iqvybrwo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3joqqsjzp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3grjreums.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uukgrzlx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgpasouc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wthmndyq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3llhawozi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjgbbsk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kuwufciv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3xzmzntsv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zbpdhnrb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gagcobgi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kxwlgvii.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ettyayyw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ifosmfqi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uifchvos.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hdyiffoq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ylqlpwvx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hidzafmc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ctqoanqv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3oyeciswj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rbbtpqva.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ewmoaeuh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wommnrpm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnspnzkj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3twbhxgje.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3exnuwyot.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ifskezym.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wwhrraky.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbvoarxd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lyzjkxhp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xwugyscd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3koromyqn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iufcqjsd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zougcbue.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fcmqdycx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hknhovdl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ytpgfzyw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3honqxlrh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3nwmbjvbl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lbbbcrsa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ctenugnx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lpnrhywf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gtfnuzpj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pvjjapyp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cfsrkalu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdwxurm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3tcppbxlq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3evbmtmoa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndjjusam.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3offrgcjc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvgdgwwr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3caibcmnd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vingiyqd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3shrfapow.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nykincsz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ulichygq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tnujjnrh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wnculiek.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dinpfbxd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3saxcarle.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3pndpkoep.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qxznyxbp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rdfxvcwc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3citiewwa.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nmtcimik.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bpphaayp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yyxbvkuk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qnqcdlqb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ctdnhwwy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dfxovlzb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3lyltvgdv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pthkjqwc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fovnwkdq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jnsewglp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pmmlpcxp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lpwwtnvl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3czargutu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tuhuylfy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pzjzbawz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uprtfeqd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kulnzegd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hwgyuukw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3qfexbjju.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jqkwbuwa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlzyuncs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lfjnzhxw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zelnvcnk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3groiyaty.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zwflzaax.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pbndbtvt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3sfvapacz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3onohgixq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gpjxovrt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjhdbfj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3threulmt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nktdiroo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3flskxwty.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbehogyh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3utvzrazv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3csxpkanj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3boqqcflg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xvpejxwa.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ztqetpod.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uljkbthx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mdnpjsrt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gpcpgbyw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hmyhgayl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hpngrbhh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3auftccjq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qnymijmi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ylnszqiv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rrhscqrc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3agjrngls.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eznrbjia.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bqqxjfxq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yskzhqrf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ayzysxpf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3efrxzjgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3natshpmr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3idrjrmzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcjahjme.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrurbrzg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3priuovpm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuyewsky.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jwefjluj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vygdoyjj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjxfkjl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gsoncixc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jmepgfkw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywcvnbbs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3naqzxvbl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tcrafang.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yqkkyjqv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sfglwjfs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxhfozyg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cedlipdd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdgifovp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3djojiuwd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ikhcuwpp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3sprwplmh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmmbult.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlqxhjqm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbieytsg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hlndwowd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tabjkzem.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zmqslnqk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3byffysak.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cfjpknas.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kljenhzh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjmjvcha.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3evsrczrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkibafxm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xhdtryyg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dgbhkkxw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gtbaxoxs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3igxqhnve.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ibesgohh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qmzkjceq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fnmlpzcg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zmzarurc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sdkyfmeb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3avrqvvfq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jdaemngv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ngrmxqbz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bmvmeqnh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kebnugtu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jpiqzkfi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3acycbhqe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3llqedsxk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vtebgnpg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rylaokfn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pyixdpnl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ptrnlsks.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xkdcvuhv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rngmodhu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bspqkyat.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qdlqdjvq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mhbqhbhu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rchhvupl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rmekbqrw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yzbvlbzr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3izvqetbx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kmgoerew.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3trrclawx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pgytvioc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lrsjtzgt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3lwqpyzgh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tmlrebbr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfjraegf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xrfohvbp.html


<!-- 参考信息 -->