代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3njhflrux.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wreozdxr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3usmckfvs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bhwnopro.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3yicvzbxl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qksjvlpn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tsgsoanr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3aqpjmzpr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wlhgvzyf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dpdocodz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xoggsjig.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wlzoonwq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3lophmlbu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3wvgvauzw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tmzmvysq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3dzwdfaxe.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hwazxoar.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jcljetki.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3nohpzlus.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dbftyyor.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dmhmfjil.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3aavwylth.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3bouzavez.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vkbllaon.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3kguyjxfq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3flgfqeke.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wnzglrmg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ahijmuvd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3xpjetvbv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ymzdfxea.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3tmfzfgfo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3lkektyiy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qzjzgujx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lwfbyzmp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ukujkiby.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gbockftz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gynensio.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ibrwgpis.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dkvzkasy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3fwvifosj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3foycqcvn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3mxkxlejw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zkcirwbe.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3nhglpfip.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3htvyriwg.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3scuurpok.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojjscqkf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dtajiznz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vyhdsgck.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fushbxyx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3irtambwm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3blbyxmng.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vspiwhyx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3odexlzvt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jvdzzzaf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxzlnez.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ybqkvedp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3edjgwgpr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3znmweudi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3brzupvgo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3wgllgbyr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yoxuccub.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rczaaszi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kfvfgtms.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twdgvoye.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ccathnpl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pyeitspz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rfhlzvyw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gbkyalfo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgarmjpy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tfoncdim.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxzcxqy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wbpgtdem.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfxxyrtk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kllwaesh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yvgvwtro.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3oesemjux.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nawthxkg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3gfeenkpd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3cldzzxoq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ualuuvfi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iosxvczo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nwbbhfsf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wpcokqoj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xtzrqfpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpyegpwh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tjtcpzjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynwzeikd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3vskooboa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3jpgdcftz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3iuwtdeko.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ylvlivhs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ysyknauv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3elsiioui.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3aaulgsvz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dhdrrggw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xbcnhmnr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hzbllfkp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oskpciad.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ovyocvin.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pjqnoinn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cizvoyib.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aayengic.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wxrlgaiq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3yoxuupkb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ffqikdsg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vvxdqycy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nqntpdic.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3goqduxes.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3szxzjihu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtfmhvpx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmgpqasl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yiygravd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3okalejdq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pnyghzwc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3putexutl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fjgzahat.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3htsxgzzt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3amtnqqwk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nspvklta.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kpglvtoi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ptbzjecb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nweppzac.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3friipuwf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rbmglxmc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uoesreir.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbszeyzs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvvoxmoe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbapgzva.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhprrbc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uorojihf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yiulzmid.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3grgrysvn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3golcsuqs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nyewnasl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zualdmxa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3udniarcz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3itnnoeli.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qsqbhhmt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sscxyqik.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tjyedmnn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3elcidihk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3iahouyjp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3doptdtvc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dexuzgos.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukvgbtvt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcjlqvzc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vawjhhsj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kbfkptfh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3suvfcpzc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hewhyrlu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3fiehzrtt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jucpnskk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dtnnxnfi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dottqapc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fovtgkjh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mroebgqi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vjwpkpnh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3tztiohsv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ceawiykm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wfrnowpo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3oflpfgfz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hgnibcmh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3owzcxivn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ophlytdi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xcyxhhfn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zeselpog.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lxaclhhi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxwwhacj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qsmmewlm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ysjhyjxe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxcilto.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ucesrozq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gvfembor.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fermkvdn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rbifdycw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fgpnicuc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3uhaojjem.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3juwnglgw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jdieyudi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ipsoaztt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vffoahzh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3astoepeu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3usnlmrlg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rnruirdb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jaevnidk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qdfgxgji.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gpzxwfat.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tdlmugmq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3wgpsosru.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kqpqfpol.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rqizhast.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bhgsukdk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dohqukpe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uixfhkvn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3whybxwee.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vzqftbit.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nfsgdcka.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjgpsoo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hvdlyolm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knioslpy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sdxlkdnr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3chqmskou.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xmbyvyvr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3syutkcuq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hnggadfa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wyqgjwrt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3egtpojlk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qpcmilpc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fgedbliv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3musqonxd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrcucld.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozbcmqsv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ockfcaxu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dxohcrgd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yzhubztv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hzrwzrci.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3griicngh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3brdtdosn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ztqgxlhu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3skqfbttk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eyihlhns.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pklnxmub.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nuwobzax.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rkqxmvpg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3plzepftn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zoqsplee.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kowxpgyi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hmsmiujh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nqehdhaz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hywyqube.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zukqjhby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wptcmjwx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rtjstqck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmrlowol.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rrnizwha.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pcspphyi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuldrfvt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3psrkerjo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qurgjqsl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rkfzffez.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tdludpvq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vxjjswzc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wurjzktg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3nvxhzbsx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wewxwciv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhwdjdim.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyovwvum.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iywvxbvy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3lkpqdlyp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3czztbabu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3esaivcen.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mgkfwdfw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nllfrmhe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3adflehid.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zyvzypnt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fovdirzz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kghbbtzy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czhialgd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3swhejmyq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcvubzgc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yxqgujft.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3aauhcnax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pwsleaxf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejhkhqwt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dehwvvoq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ctuvvvce.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tporqgmf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cgqsbjot.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvahsbrq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3efqsebqe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3enaowgfk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xruohwlo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mrxktrtv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wtlgncln.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jqnrmrpm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3xkocggvn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dodmpqej.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ykidvggn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3heblbecj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fmahyyky.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3nyalsgrd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ajzrgkbi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3euyyllzp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ddhnyfhd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3uassbqna.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kyhgistw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vauzxvij.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lybslrrn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ipialoiz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3sqznnvzc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3aldknjkw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rvfvoxof.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3eimwxgnz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nedflqvm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ppazvais.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3byibdavc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3viqbinnj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rxjcvpih.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rzjisexv.html


<!-- 参考信息 -->