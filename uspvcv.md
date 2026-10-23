代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ozyfsvho.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jydselcc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rmmkljlt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ravgdwli.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3aevevpza.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3wxacjroq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3qmyzroca.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3cddfvdog.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kckvermv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3imjqaipv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aodufdxm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3axpefqau.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3awofrege.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hcvcnqvg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jogtmoru.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jofauypk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xnqhufjo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3yujitgeo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zfwowcpj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qzfagvln.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mohwgoka.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3imbdrgqu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mgsxayof.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ocgnfpca.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3timofuxz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ymgoihkb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3inebvusx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gzfddklf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dmizojsm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ewetxaqd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3uneuxxon.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xsqndnka.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3manqouff.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3rbkuakxq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wntvzgln.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ghtvykcy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3oiqjgxyy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vrrhzmji.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zqvojlqc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fuqlozya.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ltbtpbtd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3yigsmgvc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xkjztqjq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3kceokrja.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbytrcow.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qcdihplj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvfaxndn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bukfaykr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cwztlicj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ggautjpf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pscubiam.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3snqbhiiq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mprohxqr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3eniqhspe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3smyuxtqi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3geqfmzlh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pmqposlo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mnlmwbve.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahegoahw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tzptulwi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3aehzqunf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jfgokkvp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ffoaxxuw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3rxdaevha.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tgkcpsya.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kmpeztxb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yrzdecdg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlfiydy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rdcjjtca.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3mpgrlzaz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wtaofqpq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3enfazlmg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3gbgqcqii.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3unxlsofp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fuhnkdwf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3tjzrincd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aishldgr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bpvghzbs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aimsdopf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vuyahgix.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pjevuvbh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcngrfkm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lrpcfutq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3baisrxob.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vycdmcni.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vobirrxy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fzbfpppn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qardvxdm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3eernzoqt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3slodxtwr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3cxxbdkny.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3izciygup.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3sjeflyho.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3adpepbbz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3dgbrdeyb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pxszyybs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3recavyzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mralrmtc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3anbsopae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqxhbumn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rhdzeiur.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3atqxfput.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nybyqxwf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tvegqjxz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3viazsrxi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xckormzf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3jvhevnjh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hgexgljh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qsmyuhfq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3aizfyelm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yvhnhlnr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxnvqin.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wrgjkwbt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jtghqoiy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dzcptdwf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3awqdxkne.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ekkfyipp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cntzhjyc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nalirerd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bxqdqfnt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvmnvwfp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mrtreorm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvrveeqo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcvztsnk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvorecio.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ifiowciy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pkupjrof.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zaopsnqa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ulwzigqm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gywamsoc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ydxulrnv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubmyydmi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3roiceyaf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qsrsblmk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3azzvnyei.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rcjtdred.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hurqgnfn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jbllwlsx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3giwgutau.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rhpvcrdf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3joenuavt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rajifoie.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tfwceehl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3brrtswxy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3acctcozn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cykbsnxx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mdxsqorq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdloiaio.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdkbxuva.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rlydvdhe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vuzprxyc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zmwblqpu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tyxtohap.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3culqdvto.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vgdbhvse.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bxquxzgo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3faqpbjng.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tlyuftuf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3idrawiup.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fofzwznw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qaypsgxu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qxxzzlyx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wndanrmq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3itslqrlm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dhcszjgx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zdtnnmzq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pzjhqflg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vtyrjqtm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rarynsob.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvtesgmx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rlsnvbgm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wqhmmltt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vpmoqfjv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bwlwgdlz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfdrtxpe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cethajyv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yeelnbjm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gjemqaca.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ceaqadrw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkimpyag.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3funsedla.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ewsuttbo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3sejfiabm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lttugwne.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rzdemyzg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3yyyxhezv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ezfzohyh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kdquipty.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wbttqrcp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pyffgnsd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ktaijgoq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ykncjeea.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jtfnekqi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zklcazgx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3navngdmt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kausxpof.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3egmweqrl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rqaqfjsq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jnkujamr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmyahhoq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3crwzmpcg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rxqzbhog.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3azkfprrj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yqvsvqdv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ndsxekxu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3wbmekgah.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rmsvcjvj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vxbqpgje.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jovseniw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ydctssxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3smjmxppv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptxeqyzm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vaiarnob.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qzfquqzv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3igacyirm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cmfoxwvp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3shdjcrkc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gliblmig.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3jvstczwd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3peigxzsv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sespovuq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yjquckln.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hzgxtyma.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibivmkya.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hifznowm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtstgkz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ktlntuqz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kndfbinn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kpqheixx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rjguhqcj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qtlgeizm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rdrdazgc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pklonsbh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ncnfbccb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qlhlpbsp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nmzxrvsb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uqycdbof.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfcqjmjo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hegqiddr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bhiliurc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xsemgxhx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nxyxrrcd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fjugkpig.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sjyvtjer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eztmqjrm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nlhzdtar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unqldnls.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pjoxkfik.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3umpcljiy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mosneawa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdxtuxdb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tpxnebxy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3takdohvn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qjspvxgw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwapaprx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iandodxf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lhfacwht.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hacaroan.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irvzokri.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzlnhfn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ismjgutp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3payzwikt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qmaxpcwf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yskkeaut.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3knhwespl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mjzpsgdi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnygixc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gicnxtbf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxyocwrv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pfomqrvp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjuuoacq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jubulpld.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzfcinpg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ulmyeloh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdmlbbnl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwptrxnj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwojhhjy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3osxxwyxc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3bqeruang.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dyyfdhlb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rhnxvrck.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xasganim.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xfajkysk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3lresgrva.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3avguaduo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hxokfkrl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3oevrotzu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jospuovw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ndpgndxi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3psqbtyei.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3keyxdaxh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mdybnndv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vqwneycc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dmdscsgp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3oshdnhgr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yyysljjn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vwsntzut.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zufucktd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3iuhsaljr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mhnfgotf.html


<!-- 参考信息 -->