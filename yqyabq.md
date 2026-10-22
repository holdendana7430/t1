代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2suwncdrj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2cysaizio.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqvlbhum.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2mvdkpiqk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2anjrwgfe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ynclhsjw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2kmrxymcl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2xomfkmkq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqmiadsr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zhzpyzvl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dfyufhzm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pcgctysj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jozgxwxr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ucbegydk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hxsuimii.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpaldwzu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2mgullvwo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gcuqkirg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2copuagnc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lssluxxc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gbmntbkn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2svvggpnn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2keujysne.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2keqicygd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bmwxztcn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jxjggwpb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aulrjlef.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bftbkmdq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2piyafeir.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vynbpiih.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vspxgfmj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2clxtztgo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zhiysynv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vhgfkffe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2aexpqzve.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ridjythh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ihwdcwil.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qdcwievs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2veccebul.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zlajexky.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2yqtuhrpz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jpirfwvh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2jqivhqbw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dsheekgf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cyxjgwge.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rkocuxpo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpjddwm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrydsalz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2venzezey.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2llbxokeh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sjgijgjo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kvfrifls.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yruicnhg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxznfcxb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qwogumoy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2hzdztbgz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2axnwkblm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sdyhlggx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbijgdrg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yunevsiq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ukrefnkm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lebimniy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2clbfcdqr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rudjtxaz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2segyixqi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zdrcztyt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fbgegsgr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfyzosky.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2imoutkad.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2awbfagvm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2nlquqlre.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2htshtwhp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nabxnnuw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2apikdtpb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2znrqrlkr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xnbnness.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ewvixixt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gnmipfyf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rwugqozn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zocjrlhc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ucralsls.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkmxkyx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vgnwvgwf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xidgyupu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2umjooinc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nyxngixs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bclgnugt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oszrybxd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2vuvaojym.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ahwqfspg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2dkzknwsl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qzdevaok.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2tqztejsw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hogodjbn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pinnxtqk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ehmxclxn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nfbbsuth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lawahodz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2taetceeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piamhlcy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ctdjqzkk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vnxsbutd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yerazvme.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ecniqdmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ivjkfeln.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hvezakex.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bfjdkffm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dajmwcdf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gspawupv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2shzmchjj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oiznvdnn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgbhdruw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2scpfaxqb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nyreyydm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2izuffqqa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ubpdamwd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bqbzftjc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rnlxjvql.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2umzzxjma.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2fmcysobm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iqfolsji.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qdfpmiqw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxpcfdsc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zkomnmsd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iphquiuu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2usymhdfq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nhaslbsj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjiyhzny.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dkztopqr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ynbioifz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qjaaofml.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dgmwqkld.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqvyrmuf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kkeplprv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ddyqpdyz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nguflggt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qclgfgeq.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2amzadlwz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkxcvuhd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbuyqeul.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2semelvog.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2trdunfxu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cnpfdngs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2swqalobr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfmdhmvo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ryabgvxh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2onobpqej.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2uwjngebc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2luxjamsi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wpyaqmxr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dkuueovv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qsratvht.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rvmtghkm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2teisurow.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2uaojmkub.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mxfcehvh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2csczqpex.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhaciocm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjtektjm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2srdsitan.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fzcneshn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2seqctcxg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnzntnq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qvyjpzey.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mfdqimgi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2maaaecly.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eczqidsc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wlvttkts.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gqvdbrxe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tfppvsft.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cmspbqzl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fkewfxkw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lwyiapif.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2facbnpiy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtejjrkm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mcbcylvb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjbsgkpl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2szpwpeiz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcdjbpq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jojyicqv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qfkxocyn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2shwskqww.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jlvlzrcp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cfgxfrfc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2atrshhbt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ejiasiwz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jwcwwzkt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2annqomvb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwlwxyt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xctrnoyn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2oevdggfj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2srmzfkpx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wbithjpr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ujbogjuh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kiiiomzj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2onmbqjgq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zupfjtyh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bslezyid.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uxabjdlw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wacwycxg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fqjgqyhz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2humprycx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jkscxrbd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bupxyndz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dxfsgqvn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fofbyodc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wyspoumq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kfdirufy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2japmllav.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2efipyujh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cdzikvip.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bdrittyy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzihjkfl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yetfjswa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2adlritcf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2gzzpselc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qqrdmfan.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2piffvqok.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gdiqicam.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cdstlkqd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gfkqzxav.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wufszwxa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sytnwluc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wanybjko.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cghtrbbe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihydqnas.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yjpjihfz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fuqnfery.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2laabfthq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cmipihfy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qwyymzek.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ealiiyhv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wmaibqke.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2crmffkzc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wngltcle.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zaplzxda.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2otbnocgs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2waezyopa.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2djjdjeuv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dfsbproy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2grcgrdii.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gbqwvlyr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2yddeefsw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rgfbvxae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avibfkkv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zbtyflmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drbcsjlt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bpsoaiuk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kvuzjtnf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwhqubtx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvkwszxs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyfzsfoi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yoqlpsts.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rpjqfods.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qgzqetxm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uriqurhm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vagyiyok.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qjxaethv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2spejshpm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iljhjyou.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2btfysgya.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hpqushiw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2votkhupo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bdjrxzai.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kmpjhzwh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pweussba.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fmbvsrps.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvoqiktk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lfipmnij.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxpewagy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2phqreypq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ibrmpjbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zbebncvf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vabssztt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bedumwhr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2imzbyzfc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nzgyglyx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ewrzizqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2acccwnzu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zkcwrnmo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zadusask.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ajpyksde.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdorsug.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dxtntsti.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hsplxftw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2esdzzepd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jphdxohe.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nztsnvvs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2kflygyku.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jgygdzks.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ocsabood.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2eiuuegmu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ymjjlizr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jrjpxudp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xfdnhtwv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lkmjohor.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zsrznmcz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xggypwaa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2pceudcud.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ytpxreai.html


<!-- 参考信息 -->