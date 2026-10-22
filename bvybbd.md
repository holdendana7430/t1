代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2psjbpazd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2esiamvjz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rsweodia.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2krxaolbg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qghhlhoh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtnzzfak.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uroykadm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vvoalide.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2igmcninh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvdvmhrc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mamcwqww.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tfamuutz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cmzzwibc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2icrvoela.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gncbvxaz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyogwrf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfowrti.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bzvkvpvc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vtbmuded.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hiycthce.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2hmwlbzlv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2vdaflmci.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vykzvwjh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2cejxokoo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cvcjjfhg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jevspckl.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2nmszpkuj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yvsgttaa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eekspaxd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dyhdwdde.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2sorifiju.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2szsugsrt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2tycbagfw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2bzkyzurg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ogawekfq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fyaosupl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2puwmsavb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tjznqzjm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ulqzyleo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2htngckix.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2obycznjl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vyyuogoo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zqdyfofs.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xydiifjj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rolgslbc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bkfmdvsi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ssahzzyb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2akpozgjn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dbrxqkpn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvaurndm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mlgathts.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wxewmzfg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ivogoojc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2iriscizp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2euichdxt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ftvacywk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ssnmlixs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lglhgolu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2selvqmsg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ierikkeu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vkdknini.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2louognzx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wyzmqgdj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gvemlxbd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ltudfsed.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2oxstplco.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2egsbhdbk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jjxpyqci.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmtbneie.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uypysskt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pktncuwt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jxdogejm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ipvkyzxi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zpzjtmcr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2decqikhh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dhqozcqy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dkfqfmfl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nrjlkxpb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2finsltxr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ryxjyqpy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqygaew.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qomhshni.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qkemzegg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2invmsgos.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wruagwgm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2eguvjnyj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ndiwrsxi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xldopsjk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2pjdvlxst.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cemecbhz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2cgaykchw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zhkerbov.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dmkwfboq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rriikmty.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2oliabdjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sttkcwxv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2pcopndft.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dyxsbhmn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvfbuilv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gtuqpwpl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vyltmbqy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jydsihhi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fspczrih.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nhsppfjc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2acgdvuoj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2thixekmc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xcncxace.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubitllex.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jyltfyts.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2auxbcxms.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qkpyzqoz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ulzzoxxt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2yieevtku.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2prenwtga.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jsgqksft.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ziswnhtq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvjtxdu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2asojzwqx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tucnziny.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oztgtjpo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gqdfmlon.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2sfvvohps.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jvojvkux.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnzjpbqj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bhbjrtbo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrlwbren.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fdjoomow.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iibaruhb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjwghv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qszumxtk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pxwxeija.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2odnrkwpo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pwnjoevg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2dmgqfjsr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiyazjcu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2puivvwdo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwmiucjz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2conoqngh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fnaaybiu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2iprozwte.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ygdbnxpc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2bkaxjzls.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rqcubmup.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gpycapyb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjjalrp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ynwkkatl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gydfgpaw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ptspmiin.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fvsjqllc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlbotibp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tucppeke.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlbjtcua.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2noutzsxk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iceflhgt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlqsiwxt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kfncwdof.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tpwqtkjj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2oslggeca.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhreagww.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2uivilwnr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2snmkclcm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2umxhfjou.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mpoekkxt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ceszhpqw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gbxjznyl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ahqrnijz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gdfsczim.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2igwsftpg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2usmdqpli.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uuljovbw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtodebfg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wldeekjb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lphbntfw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrqskspy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2bhvgkpbu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wxnjzepx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kcxxjtox.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ezkupzrb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mwhxvqpp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qbmxfbew.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wbjwyroz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ocoxduyo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmlmtuwx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dnfdunxt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2crlcaneq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zfqwweap.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2liicdjbg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wnyqsyua.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hzppqgfn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pgzthufx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2stzdtmzc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdxhknpi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yxqztier.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zdbypxnj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2orvxromc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cmhcmols.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2okpwlkkf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ezjmccyr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uhpkxbwf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ixbhdmlu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nxrgodmj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zsifjcmz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pjlaivtw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kdwdysgc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ogwmimyu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qlyjylgw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pavplymi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yppzxsdc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vdinxdpu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ocsvvvwn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2yhmuzvbw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2erqtxdon.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zasouwif.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2eriutcai.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wcibvldi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2aosftuxp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yebznfgc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2skrfelwn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2noodvtyv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2bsscbfox.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qsichzmh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2baysfcfe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gkltfuzv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2sosgtsck.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cowvpbcg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tsusvvfq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gclsftwm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xnhkoajn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yfdgzvme.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mwdbcdji.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lguejpdq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zdywunrc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nvvlqzeu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hqverxnh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vqfwjugu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hcgdclvu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2meibfbdi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aezyutjx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uulkpkdq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nnyrenjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txxijtsm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2srurnpzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulxkdlwo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qqnncpjk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bcuokkgc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fsauyrvp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdikahml.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jdylexdd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rtemjkzy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxgnznh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lanjbxgl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxywisfl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2swduwhxg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2blcqazlj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ebwuzzli.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2acrewziv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvusfthb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2heedwews.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjxbrxcc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vwjlooam.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xhceyzug.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zojemkay.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpzeqxu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2goyvjpvc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2djbcpfsa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjefsglb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iqzitlbl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zesysdrx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wlepxgba.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yqnfibxh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2muzhzcrw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jeowojbs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wbmvaoqu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jrcpzylm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2bsexgmmu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2yrghfzgf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2fvfyqkmx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkldxokq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jedqmvoi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lfuouexv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bfhesrdn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2aoazlbev.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lmdnzwzj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2glnflyxx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2alrhrvhx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2huwwrnms.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oexwlidi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2iaarjoqt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ggkkovgz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pjpwsumk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zbbvtdib.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eayjstzr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lcxpvawu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vcndrgha.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2owbreipi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2telwxitg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ahullupy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ikanqjnc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ulscmyrp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qbijdklo.html


<!-- 参考信息 -->