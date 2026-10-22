代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qhpmnidr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lvtzzyqp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jsvnhnam.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ntbxnuoe.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vhstmoxm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kyxfmkzx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oynibhyz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfwklei.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xxzwlhlf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gughysko.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2sawrnyfb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2cmbcjedp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2kuszmotr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2gpzeitov.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ygypmumw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2szpnkctq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qmxjjpze.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xomaoavx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cesvbbpo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wvsxilpk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ysmsswgq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2juuqgfky.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2yjhzylly.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rsjsqspk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2erckzzcw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ozfylhsm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pupcukbc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ihlgjjzy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wtgkcgnz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2qakuozbk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2xicgbyfs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vksdndzv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ioulowcf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rpnjinan.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kawcpaxi.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvodsfqy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lwnazhps.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2khyrfssy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2drwlqzya.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xsjrobgh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lalhqmzi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2edtodbrx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2cwgndwup.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2njwqodbn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2eloklzyd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uzavxzgy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmqeqafm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ucauypvg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bhzyhdyq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dfgrnhzo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2vidcjpaw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2esvwgour.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2flqjwdyz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dagukwtf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wricrbdl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2swwwusuc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2onxrtblr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dsudjtaw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lamdemgh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ndaddjad.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmwtujf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2htkvkfhh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sgbsmsjk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ckfyemce.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2tntmswed.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2dojuirwp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2clezwltv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nwqezeqc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2nmbrrufk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2asviekee.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aehrhboj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zljngdwv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfvbugsv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2pazozrch.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kzzuqbhx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqaixwxe.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2cpariepx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qfcgwfuu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ahmtbrgt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2unasujwq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qebasmft.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2agxpekdb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hwdxxgmf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jnolgrat.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hojmluhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhovtogw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2tikkpxkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2losxzqtl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qrimbqwy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ekacvzif.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2craltzud.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vsaocqjj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zgvggbdr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2feosnaqw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2riousfog.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zfkxyavw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zujsejfd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kptyctts.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oijasqxc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rawfjwut.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bhskvjwz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pgppvfxn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2slpcyudp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2feoswoer.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rtbdkbrg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2heselbqb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2latfmoru.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gwcehcte.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2naapzeap.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltzxgqsf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hyiwlrql.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2galydvcr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2agchyrju.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dmpevbih.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dccuhxak.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dtcdntmv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyjwyzt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bipvacdb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ncdljvax.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nscvekgz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yypiiubm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2odhuhhnz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lriicjbo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyeijtdl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ifkasgrx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jhykfekz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuoruzca.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rkagvyso.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tknonbkm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2szxsigqe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lecukvxf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tshxamek.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zhqbgtny.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zbppoxgg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ddbzgqtv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwounyg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ludwpniv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qmelqloi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivmcyueb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ribozprm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2cyljuwzk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2teteedcl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ejyvnjqm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wdkhfyzj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kczchqvz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2roiutjko.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ummarzpu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mndkxtft.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2owntcdka.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pbjnmsif.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2flnqnaeb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qunanmvi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ynvdhvoq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ahobfkwu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hvsuyydi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ziydrutd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2akxglkwm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xslyourz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2djplwbfd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2odkxifmn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nrxjmkiu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2irgfylzb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qpbfvpcx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bjmumrap.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fmrgajqj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oylgcjcr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hkgftxng.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mswkssoo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zstfwwoy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2smanralr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2psibgisx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nacujrvq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dnwymduc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pbaflrqu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ahmrduse.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ncjqhamp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dnecdpbu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2udmiuubw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yixzfotk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2glwrblfr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exnfmbup.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ielhscbt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2shdcoezz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vgnupeal.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xxstiyqi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2suszfauh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2fgweytda.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vazzyjgr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ihuawxtk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2dmuakxlr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kcsiaatz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ixwxrafj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gbqrcjqf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjojllcg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lfvcmgau.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zbssjupv.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lpiotbpb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rdfgywqs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2pofnfcoq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sadojsxa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mtwfrbdu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wwuugyyv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2twftrptz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2howhncov.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xcahvfaf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yqwslgdr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kclbrqry.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lviinhun.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ozuofhol.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhosffjm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jphhqmsg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tronaahp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcqjngeq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cklbqloi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2publhmbk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2pvygaojm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lstgucpp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uyjnqxsq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pzclsvxs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2girhngss.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uejqrnrc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rqgjtwle.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2deyuywtf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2awziidks.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2fsnjyxib.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2pulwtnwj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2otmnenbq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2squiznlj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2faznrbjz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nwqdeawe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pbdtijae.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2antggyal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrelchmg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mfjzxqjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzffguwa.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2roxzfcvo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2owqvicsm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hbufrjva.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bttukxnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2odqytojy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aauwzpfx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qlqwgilj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fwhpljiv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eqnzlvci.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2srcxplfp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ikjadomm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnckdtli.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqppwyc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ovmptksn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ndpnieuw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2siqxreps.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wtgrohjs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gmetmvzx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nsreedhf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vuknwxeg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2deidalgu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ikxriphj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mojswpar.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zgsaprwf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2egoiqtpg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2czhbgltm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2asdbisdi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2xgahrnum.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ohmjdscr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ldjardiv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apnrjjqh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nksryekd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rwpgcebn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rleenizr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nksjhcsu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhovwvyx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bdujmyhi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ggbznrnx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2uhmdzmbc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ihptbzfm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lzxdybsg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ccrmibnz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iuuyvnca.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2clamvakq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cijrepgp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zxbslpug.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2gpyfiycs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2bjgupjhi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pibleyvf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jbfdtqjr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vnlbpgyg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bsweaqll.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kbydfbna.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwynaab.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pvzsjafm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wowoylgz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxfvvgap.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cbhtxtzo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wclnooog.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2sgwyozts.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2fenxqlqs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2frawjyqh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2brbsswtg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kkrfcfvt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fxntqkmf.html


<!-- 参考信息 -->