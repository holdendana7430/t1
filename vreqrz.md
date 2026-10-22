代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ipikayfm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2utcqgysr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jnzwkxwj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2andhnion.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckngvetv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfpcsuzu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lghukixc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zojnmjwi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2odqjjozn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mbxgebxe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dmacnytj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tofaellu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2pouwljyf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2temsympm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zrvklhtz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2agqqjerv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bksvwqzf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ovqyxery.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2csgycshq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mgpwpweu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rmrtthzn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2wavvyewc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gqqfmjmt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nsxrcbmd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cdvegqnk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aqjkmkeb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vwyvawsd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nefvvrfp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eyedagmt.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lfcesvns.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2npwcpazx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2tdyzbhdi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jgiyskkp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gnsaxagq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cpgaznzb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2utbzxhfs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2gruhtrsj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2yfghmaui.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2lbvitefo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2iuspqrgh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2flueclzt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nkblrejd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhpjqczh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zebjsgzx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qnrxkhpr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mmzoimmj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rakkmaqg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2olwytpxv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ebnhjkrc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2noezmean.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tptgobfr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2jleolblv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2grldbzky.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ghzkhwuf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2gwfmyxvd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2btjhhrfs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wnxjxjma.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uqienvzg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ctylnoue.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2iqrrcmga.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hvajfxei.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nzpynbuq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2slrnyaqs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xobmtpdu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kmzzvapq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wydzkhtj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lmupywbs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fftjfvno.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ueotmxzy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ijqfnjcm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tapencld.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yxthlldi.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vctwvfiv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kikcfwby.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tiujiukc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2skkklgcf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ffbttldg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulnqeiwq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2eccizatw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2gahbepmt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wvlwzrno.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hivkevrj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xnusorhm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2stuiufxx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cadmyhrx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qnpnurao.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wswulcjj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bbhmtqke.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wjuahhbb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvcmdko.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qmekrujn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dufwjgas.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pgsigvbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yoqidthf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xcgfjpvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixmzjzuz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2egqcbrce.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2tppxlfwr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oihxkzia.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lxrbvgmj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tyxpjmkj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2voubgdmu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hqvxjwet.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2obccgere.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tuxecfxb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2olbkuadv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2yuvpnvwu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkbzrqsz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2byumfhzx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mhysslzz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hjaszsrm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hapzsgte.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2osdlhaih.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uxgkpnra.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2izqwxavu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hmvzxana.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwpywzh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lguvmwan.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2immcflqv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gigqdrzb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eaphltfg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rsjooijm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2asjvrukm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xwugdctp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qwjcsspk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2puuqimki.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvrllbn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dhpityzr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuxvehiu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2npatassh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2atvsvsiv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnmxcmbk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pqsbwyxn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dfqaefzz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nhpwtcbo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qvcwrmoq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqdqrxkh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvxmmtzr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxtjxgrg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qgwdnyxf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2szsdynoj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xjnrqowu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pgmvadbv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lxfjmqax.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tyysisay.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qgijccoo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cnorjjmv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ukrqmymx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pqjsjmck.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2juqcradr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nvlurhil.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2stdwbrkr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2grsmnsml.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gewlvwsk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eucrmplz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uckduzgz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2zchhjsjq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2tjyiowfg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgjyewwb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2fuseoqty.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2oswsxgbo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ivxfrwur.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2elfwictv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yofrskve.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2enayboar.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lgoikyxg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wdhllhpn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cknlbffv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2irciultd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vudpmqcn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2efztsbtj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hyucdraz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zquyckop.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylmhmkru.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nujafhsr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2glhyjnco.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wicjslod.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zbamnkah.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ahfrdqym.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqoqlsb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2salolcpe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wmfhhlas.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rvgyzlxy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2uyexnjaa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nxrtmbvz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2fwomvqhd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ngezfakv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pzeektxn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zepfehhb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rktumgga.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2snveerzk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejkyqkat.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wahbfxei.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bxksozwm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mktqobiu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zwrpvctc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ytznxeau.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ipwfinvu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rvtvzyjh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mnfimvgn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2trrvzpzz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxhkwuzm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ktfwrwqz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ezmmimjm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2joziqoax.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ypydpxwt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2qvvidmfd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tzgnmqnt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdjikhpi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bxawdika.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2xwgkabgm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2sgezaixz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nmxzzdzc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wvmpevly.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wsddvxfp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xqjscflq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ngndzcue.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyctdiny.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eulpktjk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2pttvwxgq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iefgizgi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kvrqugkb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wynpzmex.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ckryhdkc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gnrohugt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2godnkvfc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jamntbww.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nguadhlg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gamsycmd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ppegenhc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2recdnzan.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mclfxopn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mrbfgbmn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvfiqpst.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2czwblocc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2imbgkeqc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2haubgpnr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rjvpoejl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vkyuriyn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xgtttoxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxqbabch.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2smiaduhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skudvcax.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lzwcudux.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2tjcwsrlz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2geikvltd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygoasqqp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dvcvvohl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2laqfowfi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nhzmgojo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbfnltrt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwjaazqb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2imejkmne.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2sbybaelf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zcwfhlnz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2skainqgc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtqzyjlt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jdxixtay.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jekmubmd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xexxrhcv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2odrshefl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rokswxee.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cdfgnnoe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vrapahgy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jwduofyg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rinkccln.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2moiaellw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hzyihsni.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hexhqbld.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mijoonwz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2evctyokd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqopsoeb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uppjfykl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yyqfwhrc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vghdutnq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2srijuxdm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nepkhety.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hngjmukm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jubdjmyx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qglmjktt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hbstchfn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wturybpq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ulkxgtuo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pahdrusx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2iktdfjwc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nsracqek.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fyzfwpsu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kukulake.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nsgqjtge.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2koxxipuj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rwxsmogd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gyobdnvj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dhfuymny.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mvlvxara.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cpmusmio.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2adxplimd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dlmibywk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2suoziqap.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2pxdpcxpz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qzukmllz.html


<!-- 参考信息 -->