代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xlvxchmh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cwdaurhx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lfbzoodt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iqooyhro.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ntqwwbxk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycfqjaay.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qecwajhc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hpqixngc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2usmffeuw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2qgkwitvp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cyouiirw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2czpltdql.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cyndedpm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vuhycnnr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zncsdowa.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bygmaenv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2fyuvhpou.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2fjmabdic.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nrvzfxsk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ziidyfud.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bneasdop.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ifxbjcoh.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2iuecoogh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mggodrck.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2almzjndc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jzkykqyl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mvmuwqkc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2glhallvq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2yylanges.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tdqorqyo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ipsrppxy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2muncvndz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wfiaqczr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vwfbstxq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ddpvmhib.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2sbitygps.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2acjuicgn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jscimsig.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ptjgembq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlmdjkq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tuppbxul.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wcufondk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2debmsyzx.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2nyrngurc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jvwwbbxa.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2igdmjszy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2pzjbxvpx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2aqfxllkg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jmvfsrxi.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pxngaybe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2oybbqwyc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fbowgbiv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2drvicqbn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nnntbzxs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vjlmzplt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2unzhwxku.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aqgunnof.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dsuxsuyc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kbvolksj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gdqjbquz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hdlwgwez.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lkpliigg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2cbjzyxwv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vdheaycw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2irujlupl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dofbukas.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hmwhdqie.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2owrgncvf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ffucpswq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2txoshijh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yqwjypco.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ekzioyma.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qnwbhocg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2koqpcpsv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjeueou.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrrgrru.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyylcmhu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ovzwzhmw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2yqcsqhur.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nffcyget.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2gwlqvzlv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qbxjxbqf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vymtnwax.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qgxvfrky.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xnldvrfs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrrbcqa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2japbuphu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2lfyympbu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnjmqgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omrqycdf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lhatjrnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2beumxtmd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hletwplz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2iutflara.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lirbpchx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tnrqfhbh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jbiebtbp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dnnjrvpk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2slfcfdaa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ctyfacyp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mkdflqde.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lkjxdqib.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wzzdvglb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbbzidea.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kqjumqbi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pufedlix.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mrqiyuxb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rrunrjtp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oupmgkjf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tvldnlte.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qwjsjuez.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rjvapeqj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzsqmlam.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmoyhhwi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxxoxggx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2biitikks.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yrqlasxt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2gezrfevt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2eodxqgad.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uahnnqmm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fyjivrbk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdcqekqb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqfugzt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yybphhfb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lypzvcff.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dheiejro.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2htaukxog.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jreabupn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pksddsuy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ryrcfcjh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2shcmmwqq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfnysaqb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2snexzqvr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgpllxer.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ntbihsmk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwlrpqt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoocrzjv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2sucpadys.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zussnnkz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2odpvgudb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tplyudsx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2eidskwoo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2trvywkrd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vkjftnwt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sqmnkxcx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihiigkhs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2iruyahak.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcqwpyfz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrtnpezr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2znwpvint.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bxutcwwg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oieliynu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ijjgougu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2aodxsckx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xjmzurox.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2swhzotgv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zqrlpslk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xcmwuphe.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wkxjinvq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cvxvdpkr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2heyvwpyi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kfbqqkyl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tupuieoe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vugfkekr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2agtzegia.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwhbaxob.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfkjmnbc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pebyrmbg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvpnwroy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2egypvnps.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2inuubwsc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dlysonaq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iskzqgse.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jfqvlpaf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2xkhftefv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fwfwwjlz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hyjffrpo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aounxvsb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuzmfawb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxontmlc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vwhmpira.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tcboacag.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2yjykkfyr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2epggnsgy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ddpweagl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xdydghku.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2afykxzam.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2npavfrsa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2icpfurcf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wmpexztf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2debdyqcx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2smgenwwe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2szergaba.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2azzmiptc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ubsdsunq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uaphnqvh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hjkueynn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gekmmgnv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ztfvjagn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vnkmqvff.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cejkkdel.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xevyrwgv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqfkmpd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2deiduglq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jpsnmods.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mbaeogpg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2pcbdukww.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2smzujqkn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tusbwcfh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2musyordn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2pjiusqrv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zwxejhka.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kegfdmbs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2toxdrodr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mgaowcrx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yssabueb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yphjmbax.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uggnffki.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wwqhmttc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jqqaiopc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kozakxzy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qikapqgd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ksidjjps.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xjlwjtkz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kvstbltv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lqtpptxu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ulorpkcm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2shownhnq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2epdeedop.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zqltpfry.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vhjhohlc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fnrtbgzf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pcroityk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vqtratxw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lhldejoy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wmgodkvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhflgtxj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qqnlamfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyonyllf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fchthjem.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ovxuwtpq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hoimzboa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkmbglob.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgrmfgge.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gojegxgp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pjayaddt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mgxmsxhp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hynorfrx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jywwvoaz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2macvbvbf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xolmayoa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrcbesqr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zowkrmjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wqfjhuaz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjzvijfn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ezjhkqbl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2eagqqult.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ydkhwqxq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yavclsbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jbcjqjpc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tytmgswt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvokouxr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbmzyznt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uardemmr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jjjhbqay.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2spzrpivx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ksjxqoyh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2syyqspnm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2glcosqua.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwhhjjif.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gcmcpstj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dgwrctem.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gppotmyt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvedrex.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mkmsyyba.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bvdhoqji.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zcsyppss.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2neyuamia.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gprcixvm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2erswevdb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dmdtapxg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sqjfijtj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2icglizqy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2voygprhk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qydshpvr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2urozdzrv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2arlcnffo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2siabtfgx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2giwadpap.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2blworbdv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lrisxule.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ddemxsmk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rwrjnbdm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jostebrc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gnbryrpe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lefcmzyx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dxuueyzk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rqvdlyik.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xnxkqmap.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2djytgfct.html


<!-- 参考信息 -->