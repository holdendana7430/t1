代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3resdmukf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fcqsnmdz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryzheqwf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ylpeepxk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dwxaubtr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lizhfrmd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hfgtfcmn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iqrafxwl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cwniysln.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sfwmletv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cxzhycuy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3idescptu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3itdlqjtk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gazdnckf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fjqpzobl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wouwqrrj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vdvfjaie.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3uomdxzlg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3lnsqxxgh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kzxosipi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3rqifdzud.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ztidltxi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tienjaad.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gsboipgx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3doqzcktz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tvcoftie.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3mgqvhlia.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uhfavhbc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kwixotls.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dfgyluvu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3hiivulfu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kadqpmsz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zkhaodap.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ubszyorj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uqmlnmfm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fpfllxpl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgacily.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wcysrxer.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wrolxoby.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3emwmyqgu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3xzqzsgkn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxhqehc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3grekjpxm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3oinrgrkk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yoaruguk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvuyehw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhmuift.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xgglzwyl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jqeolwck.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3akysbeae.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ebmannkn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mihjnjxr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3urawlvmz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mqkwwetr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3edafrgut.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ceffblbr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qqsgqiir.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uafwvyvi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xplyelml.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3parootzb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qhgvbyjn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mxhhmlaf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vktoyunr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3coxnyfrq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ypwndqnf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wyegotiv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fhobtgus.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3chwqnsvi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zhpypltb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tdlsdtwv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dywqijuz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3sjvnxavh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3znyuqwem.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3awoqjhkn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gmxkgagb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jsuzchmr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3oxqbienc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fptzxbse.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kendcsji.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oybwetkb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxtarnpp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ttqsqgmq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3iqamnrbi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3tyxmljkh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mvlmcgaf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wtxqlbsm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kafjjcxz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vxevlxhj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pvczjvnx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nvxcyjem.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3oigokvvs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wqrtxzjg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3utnkoprk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peafrrca.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wzhopsuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkhzalad.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qorgftur.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rnvfxuuk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mjtdoisr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3osggrdts.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zfgbxvuu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3luivkrwd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3gqktpwpm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ytfctkgv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lcbnbevz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3nbugjkjj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yxfmulre.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myyxmjym.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gbuykqoe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ravkhdlu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ghjdqirh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hdwrfdir.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3cizjolnv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nzmafkig.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dnphpqmj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fuphtnna.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtrorozy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnvhqprr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zfzpqzcl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgfncoxx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3soubacxr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3bhoedjsw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ccsyibvr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yvooanif.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ypdxjmre.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vpxtngka.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljidrzrt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3usarpyai.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ekgzohqp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsfkqjsm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ctpmswgx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3engwnxjc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3urvrgmtw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zybpwevq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uityvrnm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pethonoo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xczttxfs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3svywcfgc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cjsoophs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ldmybmrr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vkkwddpk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3boapysel.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgqgxva.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3eymunjap.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrwrdnbw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aocxrbpb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgdtuctv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3orajwcry.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pxnlnpjf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpdjszeq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jjrlprup.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3enkorpjc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbgnngob.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3firhpoco.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fanzpgeh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3grdinlld.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3masggaud.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wbnawczq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vaahoony.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dyryhefp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3olcgmwwa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hybrlirn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ueslyhop.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3efvurdxj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wrswvjdb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ypxzycln.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hqhzapjt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jqynnpgc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mldplxce.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3uerenwwk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wiczbvfz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3otbcqwrq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbmlwbxh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gojytfsl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xmsofofz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rmghjtkf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wavlrdjc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ugfyhkfl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ptdilaot.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjlsheok.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vtdlrlcq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ysclcybr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rfmzkhxs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nnvwtvsu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3obkfvqkt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbvqiziy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pypaocht.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3htinowqp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fwnlgkza.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3esndanfc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hsaqlyvh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gelktnzs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ulhdwhxt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dgnpuabe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ghvyykjg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kwdwjfmg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wsswgpmx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ahcshrrw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mtttzqgw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yixfaiww.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dokuafgn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3gxxceozp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tqrkpbkm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bjfypxoe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3evxqlhkg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jjjqkdiv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wtgxtlua.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3egwriecj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvetpsrf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qvhqpgzs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3giybouxl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3iftpwkuj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xgqthmcj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qrhtgbug.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fazwjvzr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3sogbhzup.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bamrpvdu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccczrnjz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nauzfhih.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fddbwzoc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ucgfnrie.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zdscxaie.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vhutoqmd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jfopclxy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rzgtftlf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3heafkczy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sfcgzhle.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tshdshle.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bpeqrjah.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ntqgfcan.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ecwkpyhc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3exmvjlrm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mwrumzuu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3muzodvgj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wiknvhcw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pqmphvzr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fxigmynb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dkolfikj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3uftbmgxj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3efbavztl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtdguvoy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qtdlkcwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tguinxyi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwfhixas.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fkmqwbmn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ylfvkhsp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nwtvrvkp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gedgcuzn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahotuppy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vltfcybo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycdprclk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qxiaotxp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ytmmrhnu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3imgfhhka.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lahelwqm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwjlywey.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hnciqxaz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3iqsnplrj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bznvpaxo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3pzaoowbm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bunjywnp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ywqjoxcf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3frehrfpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jztxgpbh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ozmwstwz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhawzbpo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzjmwbrb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hcfdcpvk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3poaflfqx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hhcrruky.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yurzjvdf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3epuyrqqv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rfpcjxmb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bvppxzyh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wgnqubjz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pgrdwmtb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jltvgami.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kqiyxflr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nxvyipui.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zymhqbhg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qdvokbez.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fcxdhlzp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hybwtagb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mewzpbbl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jjcxiscn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vkpdttvi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gikbubkm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qlxotzne.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jyeuprsb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3futoypff.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3errphfuv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hhhjxinv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ykkltcar.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pykkdrbs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3uomfybiu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ipqsmfrx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3smpntmki.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3saanjkaw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rfrpgbhb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwmlyllb.html


<!-- 参考信息 -->