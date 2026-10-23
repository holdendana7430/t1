代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pwlrroia.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfttpngq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3epxfqinf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jaxkgdrr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3csthjuyn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3srfdgepl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wptuvwmy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpdsozxg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tisdbjlu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ciklzqvh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3phqwqhdy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fctquwvr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nrirqezx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ljetayyr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zpfthslb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3zmqdkzxl.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nmeqapwi.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lucdgbir.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3smxrjvup.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3siiqmtzz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nnjnqxch.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dbstcqzw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ygsauasp.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ebzsaedo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3osknduns.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zycvsdvw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3cdvfkzpo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dclzhfww.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3daftgshe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3ccnwautr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3emvssrtn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vdvgzzsx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3sxdsybfe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3iovzbdlq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3bdasahrp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3lyxyaenk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ipkdgkiw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zcpumcil.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dxvtpxzt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lwllrbpv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uerozqih.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oyrsdich.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mojixtbf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3miuzjpkt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wjpmcich.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ithtjicl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3afrvnmgk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dffjbmml.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kcolfady.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3txokvgtf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ftlpxqmo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ubkjoyzq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jhloubxc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eqpwhtjd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jkyvvjiy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppsbbizh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ybumaigd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uijkigul.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ijmqrqrv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhaszhm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iydevhmu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lmnhfxdb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ismfwymt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vyoemrpl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bcksadhi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3useyjcio.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ziiubrac.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mbxcqrnh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3gdxymaom.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3oobghbrp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3klnqsowx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tuvfrrvq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3hndkjafv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxbhlgol.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbctlwas.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gizemvjs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ypdroful.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qigawpbg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ilqegpju.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zxvnibox.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3dncugnot.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dscpoatt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3nylzgycp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yryhcjyp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mrtsugnp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zespezlw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3pulsncjp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pmzgabaj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3itqtetld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqbfwgvb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ilelxkeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksldnnak.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3sjnfmtgg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3tbvjdrva.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vivnzinm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cfborrrx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qkhntojm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3unyfpwml.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ccsouomz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3zmhdomti.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qczsomcs.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zdmvcrsv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3weepnwlt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pimdobuw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vnouevsv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cvpzkqrw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tlrmvydx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vduzrkhn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hsjjarih.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bvawjqfj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3egltnmcy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lecgunff.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksoximal.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbcfoev.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ukencnth.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuhzzunt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdifgfnh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nsrulyii.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bmvtdveo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jhqtqjfb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kmadvqyp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogvqwdek.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndpwsfru.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xhlmbovi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zfumxlfw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ajncmpvj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3lscbcvpt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ttnpxcbb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rzdqgzcm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vszosmhs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihmjymas.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mssfchtl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cmfaitdh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcpxapdd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qjltuwzg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pwzsggmv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3feegbceo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3awjkkobq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kmceodqh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3sgbaszbn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3msodnpvr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hjdaqekp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkfkbzgm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yhaueztb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wemdiahk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zilxhrxj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bvfeuzzv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3suvhkivm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdkpmkos.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eomnyupk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qzmtjywu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3weqsiido.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3oqfxqzxj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3prcgfzkz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ispjdpbu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lovljdnv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3tcduyuac.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tzjmelhx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3olybbeza.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nhswxeiy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qicurbjo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfvndaio.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3amrndfyt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mogzshyp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fbzzfrmi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qlpddlcz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xtxljzoq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3njjovcrs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bmybpbse.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpjbckrr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xtmrftlb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wdtwyryr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmchsbla.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3nhzozeyx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdtrsoh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfylkggm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pjysffcc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3goxnpgtc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ahjvochp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rhfbzvod.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3jmkhiyre.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyarayqk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wzwhxsdb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3deogqrci.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rqopyyru.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hhxzvxsn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tnbdzjef.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwiwwznn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qjfaqutg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kfkzefgt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rstodkab.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cspdnuoa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3atdmkjny.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ujokujzs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tpztvowa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ozgwkyaf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fvksyedh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pqkuwlan.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3pfhyelin.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3aelztpdn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jdljzehx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3eooehjkp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qsxlpaxf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nhjjaefi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3edxhdstu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tawmcxad.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uqnfjwae.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3usmneqde.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vjuihwjm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3maxcixxx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rkcoxxys.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3bugjsahl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rdehbvea.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3efgpehez.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmorzux.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3przrjgas.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ohpxmbre.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhcxugq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vouxymhn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wmtfuetk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zsxnuyin.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lklhqtwj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swawnqqo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zonpcktp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ohdcxjwn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iggvmwwc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jbtkfqyx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ogvscgkj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3nrikqrya.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrrsitiu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jiakpxpk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cfomamjo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ikturbkh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3iwibvquc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vbcdhcgy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ftrqwyqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vciwwpmn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3yvxfjxsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nirjbvsb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kxelhksj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ghrphslj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yovxrozc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jhhkjxyu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xgcjfmaw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdefbjly.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3goyrbqen.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hgzbxhko.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkvnnqyu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3stebbwyh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lqomsbwm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3toqsfwcl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jtkhjebh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3srxdqqxp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hurbyuyw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qhxrcvyp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3euqqmzob.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qsscaipi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjkyydzb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dhyreulq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3juuejesj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gpuxvwjl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oghbrnvw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvocxake.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bjrojdtn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kpxdzwbj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3agwrtpjr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xwtrfpfx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tqxdpyrw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pttpqcae.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsgupicy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hdhfbjcd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nmxxfhyv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ypdzslem.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vwkjklup.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlakkbct.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3chnmrscz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ohutnvut.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mwyfowhr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mgazghaf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3agdrglke.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vekuwizr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dqpsofst.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zrqxmzdx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fsbvuefn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3iduionlj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tqikohsh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ssmlkwxk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aflheare.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dgprnzga.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ytuxzxff.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gtwvewda.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3bywcldyx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3psvdiuqx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pxolpsxr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3qhrsanqk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mmeeyvou.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gsydgsmo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3eaxshrbo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3aoiryhqh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xgkznmyt.html


<!-- 参考信息 -->