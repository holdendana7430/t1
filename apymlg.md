代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ifacrbxt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gmpbjuoc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3negeiymw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fsnilfnf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eucgnrqz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bwyxgcuq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubicibmy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kjhxlwdi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3myrkdwha.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3oangexhp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xlcomgrb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yhtlmkjr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eekizkqy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tznsxdkn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kdjjyvcb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jrmswukx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fewvwffm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3keldwnpd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3atyszcjy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nwcmlsgb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3omdtxzvb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xrurkdxp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ekrawwwn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ioliprrl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wgggpesc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ptmzdnwu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3vluuhlyk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3sblequpe.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ssomxncp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ilstevoy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3scfwlobn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3jqcdrfar.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3veidsait.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gpvbdidh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3qanqctcg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uapdsgad.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xovmhwlp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3oxaliqen.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3uksfovxg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ojbadsgx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3gxmtrvte.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3pylrvbku.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xpltdmzk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3uduuqiwo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wvbeqzga.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bwpupoas.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3bptbxltc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ekhsqltj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkpddmiw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vjsvmsxe.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmotgxlr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtrtyxpq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnvqzzd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ghwgbsgu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3csvnyhja.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3gcfpwfix.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3iskzjmvn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3oarvmmas.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xxmgaubm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rpbkkgss.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fomiwpsm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rvwdlwcu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yeetjfot.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oqwqtiee.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3nnbgpalj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3runridik.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wkzdqqws.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zrknhdwc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nxkamisr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lswwyvui.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hllluuwv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wymnlygp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hfkcajbw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3kvprmkoa.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jtceqsld.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3gwhucglx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxknszj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dfgraitn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3evisfkuo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3rtqllvgl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ljosgadn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rnlmibek.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3crihcfjg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3blmltcro.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3sbsumlfw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbdbtzsk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3liyrdwxz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmdjcshb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vfsjrqam.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3frndemoj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3anekwtib.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ductmpel.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ikvnsmcg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3umtdwxpq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3fnodxsrb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pivbethn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jqyxggow.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eoplmjbv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3dtcjxmcq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pkkmlube.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3soejskko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvhjoxta.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nsvpoxlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nugnunrc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gppyzvvd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oxkgwtfu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkqmdlut.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rgpbraxy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pimdvhzq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nlngacja.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ikvxczjo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3glittxlv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xsheisbj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dmwjfblf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lcgkstth.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bacvywey.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3abmdwmjt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3olmxllrb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xbraeftb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3uvdtjkda.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sxwtchyz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qsqolrtw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vkmrfntr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3dwurwdap.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmwuqwth.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vkikcvfo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axbsptdi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nmxyqqqo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nbzkgqcv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tilxktbx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ikmvxrvg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3edfbnpcw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cfejunzz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3scrbjpbg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yvppnyce.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qtsagfpp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3djohushq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fspgeidf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3htrwjgcw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yqcyaoxy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ivrxcxeg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qtcpvink.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmukiscs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bhimbhuk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cbudefai.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfdvwmd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3imluwsts.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kzxzrqlb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gvvlbbsu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tevkvvtm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3foarkkrd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxccyify.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmunuiip.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rkdfkybz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozvjhshc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ytgfxtps.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kbjowoxm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xkfnvbgr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kudcotyw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrropbhc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbxjbshu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3utezsjwu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3emhcnwyg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtjnvgia.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3sedljhuc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hywlhmrr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3elvsutuu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kwabivxf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ilftsfxk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3snykpzym.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fusrykdo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zoudtruw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uwxxsxlr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pzhqdchw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zfwowdxs.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3triefwpn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3svajkphv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3cyhxbila.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vpdqhyvf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xwnvoytr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgdqovoc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cadwypxh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aizprgma.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wktlnwfm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3einnvwgy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kocxovzb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3pdjcloox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzpvfzso.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3uilpzcxp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qhkmpakk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hajdvmse.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3azfqaoez.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uanxwbqi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeiqalst.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zaobvusa.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3toetadkw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hgylcfpd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ehvuyddd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3scwinayn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lilcbivz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3uibhuteq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dgoqksvl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxprcsx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pnghbdac.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mnprsalj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xeajazst.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vdefodmj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtyhdnla.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gfxiiriq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwppwpyu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nlhjzoei.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zimompco.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zarpnxbt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wqhglpsn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zgwjvtsz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ultlvvbz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nklrhtne.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3agmrrshj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dxpnpggd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tymqvyou.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rcodtzta.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mshdlcsa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hzjzibab.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zzlcrlzv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nczcrgzq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdnxvnly.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dglvkpha.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jiccipma.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ttbnwwwg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynnkcaor.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lhtgyexg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qanrcxmp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jnehlpon.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3knidvjaw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xkoxnqlp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ngcayaqb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mlsmredf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3beuqgark.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xaoiixoz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3eeajrfsi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hofwqioc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uyvchqbl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zqejzsur.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pqyjmjpx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bjshdvgr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lvnfvinn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vqqmspki.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qttefngh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykefpdry.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tcxbrnqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnidrxzt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ogiaghal.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jlclfrqi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bigklkmq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzirykps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhgdqczu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cysktiip.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3biallnca.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mppdgspm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3peogemma.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjuwupkt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rjbkhsxd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3myslatzw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prlezscz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwsjyxle.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zdvbubcy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tvawfurf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3nmmejutl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qafgqyfo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzmhczxw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlicgus.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3szyihvpr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmotlnis.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3duzbwpfe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3udvsvxud.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gxrxccua.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ucphgzdy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ddvziuls.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3raxpnmsg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3geatkidf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zuwatkzp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hfcfbegp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xxdcdoku.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wxvzbrnm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vgebegqn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xybypgad.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exnfmaxu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tdvssgxf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3unybtvpw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3aekbbcdg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jmsjwiuo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ragmzadr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nffaocxw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xrtdmuzl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3njsjdyfq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gdkxmedl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jvktwsaf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ktgdvaab.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fdkabkik.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gyizeuhb.html


<!-- 参考信息 -->