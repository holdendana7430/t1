代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rxywcjki.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vtsrcwin.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwuveqda.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2icllqjsl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bnfepigw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fxhcnawl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2platuyox.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rldgzxkq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ojfucfea.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ccnizpbr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yjapfzpr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekpbiimo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2cuzuskiw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wodtbbno.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dolhwite.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rrhxxctk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mkuqpugw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hhvgtvon.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2inwlqlby.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ihmogmid.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gakjkrgf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2awlplqxx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vehxehow.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2dvzdpkzt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hihuqemi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lfgiobah.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2buzjzoms.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lyqblddb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2epnxcovj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2mcxpstzn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2xvghcrei.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2gflfeogc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xpuzktla.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zropiusr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wiggswzt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2tdrbmnzl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2avqgpgrc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2abaezbop.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tlhrzjod.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2rhvfilul.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2itqewhwz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dngesrih.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvtffaqw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bivlysjg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hfufceuv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bdexoyej.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pqnwkned.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hvdjrvks.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2isugibun.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2wohjhvzr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rorndfsg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2umznjmtt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hyziiiki.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2phnodvus.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2etorwtzl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ozoervzz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2owvfoeqs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cedfdbxx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hlrndtds.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fvstxbze.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wjiikuqx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2haomwbqb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2llgdqucn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vhmfxmvg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dzljzvlw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xukqklnl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2zbnhacvp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jjwuqmfp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nrlowaas.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pkilcfca.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2udabkfbq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2aethejwk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdnxlan.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vayogcgi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zalofsdw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mjhbtrfg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2yiotnoeq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vfcaonjh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jhchjmqw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xumluhal.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrgedqt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fnxsdbls.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2cyhowgtr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2laphylyw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ukqqvcjr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zfplzzyr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hpmkoxle.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rsclsyhl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rfxkutgr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zsnlpzdj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hjzmmfcz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bkspjmwv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdsiwui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgpgukde.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2phdgavyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fssgbpss.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ygmvycph.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2eofjjppv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2njrjjztx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mmxdlkpg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cgzdbyyj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qgzwnyuc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gqgarjgk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2aspvkdoq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gipiwumt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2yeehfsyc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mtyghnbf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wpqcypzq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nwutogts.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hvlzfcdf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yejkbxjq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wudnkgfd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2feauormp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zpktuwrr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2pzeftccv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2avmlhvak.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsargdya.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xmvlfyhs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njgysvcg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugbgvimw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdwjwfkp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cahfccgq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vwomsmnl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ixswfqxm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vslzxpab.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2asyedyvk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwecpiqx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bkayfonn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fnpxwuzs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qcmxqigo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2obyyxkqt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjyulude.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ydwenrjb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ehhrjekx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2jzbtjtuo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuudppha.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2puxzpjgo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kkpibjpn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lpdittno.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2cqrpzvqc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wxzfwqhw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vreqcjvf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmiywjq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjubjz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sapbdfkp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfeizcqs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cssrwlxe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hohugbdx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dhuubics.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ahblfulu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jwojrvza.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2aaztyeix.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzagjvmj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kautebyv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovhtwoko.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sdrprzbk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2idnjyecj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2asgqzhmn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bhixfsyh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2onudzdib.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vjhvyfib.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xnkcivgc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hibyqdyi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lypahtlr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jinilyci.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mwthkpiv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ssoheppz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qrciuugg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dpakvjcq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qqbrjleq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ruycpryz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nsaqatfz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qweuddbt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfclslmg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2klbvbzpo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2poxkojrd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufukpffb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2glqicqcy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hripuofh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rhfkpcoz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qmofrivq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cphkfasx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajwkbdiv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jtzljyma.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2yblsmiex.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvqroerw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2bawjeawn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wkwgbjrs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vaafbfav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rdoogwoe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2idvbvulo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aeulcitj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2oirpneos.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wflrdldo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gnughfpi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zpziiafc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2avudvlyv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2netocrdp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ocgzwipj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ksjvmpjm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gizkxmkz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hguhkvzn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ydvytndi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bmmmsgeh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wzezmdni.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2niphsorh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cckpisaw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ouonhwrh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zvgyvqgp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mmtkotxv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gxwctoui.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ddlytfdn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zgkaesgh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qsxglmoh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2qxrlkztm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxmcyjj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2znkgnxvv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdjfmmxe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aiebvymn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdkylakk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jcoycbpb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nmfiawve.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jywwkjif.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2obvgqafo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2udlwietj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gdgdmsmj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mrthqwmr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sgszgxjy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fvyufmbk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtlotpda.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2prvwhtkm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yixccaod.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2klrniwee.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bmiaugqz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sxmcwadt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gkhdmrmz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gvyyspuu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qkrllmoa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2debbhfvj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kjtgkkeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjvqnvad.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kyixmxqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhfooqxv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bstzwqfx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ehjrnxvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdrdjucf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibzvcylb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olkrzglv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ichlwyqq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2smjxeqnu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjgkukga.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyslwbvs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxnbhzub.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2irehakli.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tvgfadcn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mvwrwnez.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elgfgkto.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2iujasubz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rabhyyel.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wcjtalth.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2evgmfhaw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mckkhopo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wufdqrdv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2edetzrry.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhrqiep.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ncxwwfoj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hrliznen.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xbjesdti.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2umfbbvvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2annwwuvx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ggmfogng.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhaxghrl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2onkjvdvd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qrbwwhxs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fgmpoyla.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2epzeeepn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pvxsdgqm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klpzbfil.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wcvwgvcy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2eopgnuux.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tnhyfglz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zyoklwim.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fbawpdpb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sqgujmxi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jiptirer.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uunpuwpv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xftladzx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fvwhbgvj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2djezivov.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dgkhqtmr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2oadzchem.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzobxvvq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gllsdhcw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kzwqmayf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wvlclaav.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bkoowcdl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vtppwdnb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2llnqwpoy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cpltwlbo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rxkrteyz.html


<!-- 参考信息 -->