代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vnhillri.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ejzdyeou.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2drcwxgum.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgucsime.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2yltfzoed.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kjwlfzdo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2viftywzy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ungcsfut.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2endjlvwr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrlrrosn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iavzukbw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qpyqdwkq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dgodhvgr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkheyvid.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tdkxkkiu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2exkbtltt.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ekypwjbd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2plksgcjh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzylbpy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tcwrseww.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ifyzymil.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2egjfhlnc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2kivxnbrv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2vphfoikl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2zgyqmcab.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2gaaqbrvq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2istkuqyh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2lrpvyztd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2clenvshf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yfboilyk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2liblhrpn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hndzsoyd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mtquofms.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fvfvopno.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ithzhubv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2geismijt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lspcrjnp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hqhcumzb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2piwfxstl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bxmigksg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2hgfyvcfo.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2olanvsbc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2givujdct.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2viezdwig.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jlmwvbwr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hvkpgape.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2votlrksk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jrtofjra.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dgmwkodp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wewywhbn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zrgvorfv.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2mbgycaxd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lxrngytp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zrbgvktv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2yopuhsnj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ngwggptk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ufuqkesv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zzymjrfj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abbfjmsq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qcbezpno.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zixdxbsh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vaijnjbi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2giwvwdde.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ljeuqfki.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ksbvtaeg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2chtyhyzc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qptqdxuk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brnxqqdo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pdqvqwfc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hijzesis.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ynhvswxq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2rzcrystf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvxvapsm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxncgzxy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nluirbxl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2isawldrs.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2iivsexjt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rzphticb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lroohiyb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nkkooipa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2utiuvkcc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xetmniwi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2benofbbq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2psphvlth.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmlcwyup.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rflmvytj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2msnejmug.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2flcqlrpb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yidukdxj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vcyodund.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2snbhbtvu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2okamktww.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rcxzdhgk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbjakim.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jmdqhfpn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gwlbsmlq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwtagih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmuykdfz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fssxfcoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzkdjeqx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2umyomyrq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2clnulnzv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2beyfqaxw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hciwbikn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zpxdnhqd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ntjisnqu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2wiusdyrb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2msrutfgc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bredhlfl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hkensxoz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2moloaclk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zbuoytvo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ajxfxisp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xwxtxeyy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bfymfhbr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2doedabyj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xiagupeu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ihsqxtqr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2rnwidxuz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qbslyctl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vikxnctc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2supjlamn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2upswvive.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qxhuiove.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rmxacqxp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2owgvcvki.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nroayihg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnyokhjt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rtphzukx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdlacbf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjwhnrf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtyrfvx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2krgewxvu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bvszjyfh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ezplyrmd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gakynydn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pcfsgokv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mpxlqgja.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2omjggzmg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2obxycwcg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fohwjaen.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpdfeuzo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwejduu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2oppkagwd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2arorivvd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qjissuwd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wlqjggdd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2eubvrqwl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2salfmgzc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vilfahgi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2tyzpprhe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2okuhupcw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2reiptbwg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzvyrqgs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqpaqiia.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2dlnyqzbm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zukqhhkj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqnugzrs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjjtxfeo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2stgcznmo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2aowvldnz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajothouz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgailoa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xxiqvift.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kpaaglcz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jqgqxywn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lrshubhg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ikvwwmod.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2akmlhjyo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xyoojvqh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vuminucv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lzpcjyay.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gxlipiex.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ikiwjapi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pnqwdeac.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwwgkpji.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdfjkimj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjvrftta.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2msttgjsa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2joxnqfgw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zkbpcfru.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2redcmuin.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lcwnwynv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzubmzrh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2crupifwx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ytgqbuhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqbhkfcm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xskegjxb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hathpare.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgxfbnmv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2boptcmzt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2riztpvuc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ovldyrtc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fzggdmcr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dfvdjgug.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zqihpevb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uktekxqk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2asbidoqa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zigsvjmu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dkmcjdjz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2guzadqkm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jetkmgja.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jgxcjkrb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgosgclc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vslazsew.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qxnkjdip.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mduhdwin.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2axdglxpf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wnapsmll.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2aktixpas.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2cwcmakzo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkvhwgii.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2dorppjnu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tcpmzjlg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jhgqluwy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqulmvh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2reatzkne.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ykpeotov.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mwsusbwd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2imoruawt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbvmqwy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcsfvtav.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2delctufw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iunpdigl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzhneuwq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkvpltav.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fbuqxjny.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wlwimpqu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2itajarda.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aqnmagom.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nzgsiyew.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oillcymr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ogptckiz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cpllmdjp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2smhxfkfw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gsgbjebt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ioqmxupk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvdbgtif.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oxabkssd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hmicxenu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vkusnhiq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vjudlynv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ohyegvgo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zsywqail.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rakszbmk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hwrpfitf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nitoziya.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oftmtcnz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2attvlmyw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qstimnax.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ywefphgw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uycaaqqy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fytdogpu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nzzutejd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2taiidoma.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbijntzp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kxuqacoh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cjkuckqt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybumklyt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ryfgamwm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lapcbjdk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yrzsywvw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cnvbezfq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2foqajgia.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2prxzeajt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pupeacqy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mnaiohxg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pbuqpfwv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnvlieom.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kcuvqhhv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2pzbybnro.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pekbxeaz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fypkaoxa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2mgnhadjg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2sryfzflc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2kilrgnas.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vzrqushy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xeduavno.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pdxhphnh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2twslrsku.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cpyuyvof.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqdzgwbx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zfylddiz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ukoyjlhu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ggepghdf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wwsowgcm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kgwtfpjp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vgoextxt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bwnoylko.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2erkrkenr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2celxoyhq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2gftpvbfb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kzdcunyg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ufnnjxnw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zqdfsgte.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hjlzlher.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sfvbpwgp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fkzrugob.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mluwjbwh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2haopiaqi.html


<!-- 参考信息 -->