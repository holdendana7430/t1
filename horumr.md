代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3dzbbrjxs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lxgpysxk.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvlspkgk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3juwxpmic.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nhbksebm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3azwosikf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxvzavkm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3oufgfcyt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uqbdajiz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vtmzznbq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bopqruqb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vjyccexj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3enwglxiw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3opcljher.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fhvmicyk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hjyyhzao.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3iqkulgfo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3exahhgyu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hnlvsnia.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpckeax.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dakvpnww.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hrqfxclf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3tayligei.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ztfbcryn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3tvfkngkq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3wuzebnuq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tzkagijo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3lihojraq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ovtfaybm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nvvgelwo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3zphohotm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zlibxbll.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ccekzykl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3amllgrib.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kdhgqwqi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3zkasjljn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nxnvldge.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3fuohwzpv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qazexbgw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3cnklwlkn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ptepyzfp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3tqmjclvb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3siqllema.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3opniggpf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vryofuwv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqwybse.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pfckxzuc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mbdqtcxp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gkzbhthr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhfjamm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wuuszfho.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jxzancho.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mrcveuow.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3nilngsqt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3nwxhztop.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jtkuvxol.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3uqubualu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3wsbhjfgm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3flplzlze.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bdmuibhi.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jyykjdzp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tiyrucls.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3hfuxrlbx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3prhyymsd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fbeokjio.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3hqhevssm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pojkmhjz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rtmfnims.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ubrderqq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3hszqyjty.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lewfvkcb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3apmsdtaw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehuwzftu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jnlkkpvx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kvaztbke.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3hgygemka.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3trliepar.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vymqdrtt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gyiqqfbx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bgpxxeod.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3kbmdgrsr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xyslhzal.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3njqwkosc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqtwdwne.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3nheigoyt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pveeojre.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3amhfvysi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3laxibxyq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gsdgjsmv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3mcrbghef.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdnposh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qmfdzmvg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3atgksjbi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fxdejvbp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3idfmdqpo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3jixefwfd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pvcgkqmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkjwptsv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3nvlnilbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzqtgqpy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ljwfxvwm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zvmbefxc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3geehnnud.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ptglrpcb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xsqjdccc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dzdfcrdq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zdvisxzq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3udmmyqxr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lysfrgid.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ginbsaaf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vxsydykk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3epiozodx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mlxfbwen.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sutjppsd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3unhfisll.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zcedtguh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uctgvztb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mxzcwyus.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jceatzwy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3uobjwuqn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iwwygocj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gyumdsnh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mdtormca.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3timkdjeq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xuwelfly.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ktrqpegv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ufcikjuo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eglwxfud.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hwrkkrrr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tfhmzjwo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmxydsvf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcyncncc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ybivlwcd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3dyjmhicw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rxdauskn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bagiskbh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zulabmrw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3frkenxil.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pjbvrkkj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3efpttjid.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzbjqiiv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pzupomxr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ezecgioz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xfrfzile.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3obvkiubw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bgrtwuiy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kyhqfoea.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chtsfknn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3snaelgyq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayxqaeqx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hvlqoapt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mqxkuhkn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cldhxhop.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dheznrdj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekbswpcv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxixlvzy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqgzvagf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fturuezg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3izuirnsk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ssijmjjr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wioxwjyr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jqbbxmiq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qjkgjdeq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yxoxgvhw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3nqxklueg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qhruicrw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bocflpnp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ahisvept.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tnzjkzsh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvatuykl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zsnrmytn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hcbblekd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3irhhpufw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mgelavvx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qounyxnn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3birivxar.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3suhwjypc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cxhqbhgs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqcwjmzj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nfjmciqj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3avkxhjfe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bgjsldgb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ebamjcpg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3iplojdfb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nfyxyhco.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kayaowwa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtrdloy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pirljbmr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gornetyi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypavvktb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dokzwhqu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ntfteakc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ycltguse.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gmbyhleh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tqnvvvsd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkzzdohf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ftelognq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qqotpzyg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rbepugwj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3heqleqcc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3viptpsaz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lwdruvjr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zpgdvzpo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3blkoaobe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3njemtuqv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3umxmfwkd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zapwuhpw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tbjjrcft.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dheriqiq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zcivsshi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3jxujjivf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdiwhyyu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3usteyptu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ybqttihc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lxdjiqmi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3myenibwt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3owyhbfxh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bkvizbkq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nldxegvb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3iguriubv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zhqwpvdx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wavpugzh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgxtiuhx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtyrpzm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vzygwkqx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aachcwmh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yufodcvw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tvvizxaz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ouslplid.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xaivllwe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uuhgqfsv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jaqufxzn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qlsvudaz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3asgyvbhj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qletqbjl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mlzjucxh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fxgvblzu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3oapjhvwx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vshwffqg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uzqmaezm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bffihlvc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kmnhlqlw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3edrmodwv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gddlnwna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yioghrgl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3anlawatr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkpelarm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ydpcqxnl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rvbonzud.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcrspvzz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnictajz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3addxahlh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bqiskshi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uhdoosmo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rpksvxaf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3awvbbvab.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cpwylvrx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3enkdwios.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ktemsusk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zrlwwzxj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lnniruqf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3aopsurfl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3euapniuh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3anfdarxg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxcagbio.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3aezopeif.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pkgxcvhw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebpevaxf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3myyecosz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3punrkweg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjnzjkew.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mcatphub.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3oycipneq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hrvpzbab.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3afbenkdq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hovxgoox.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hryvdmlc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhcdipis.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3btxubxzl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3otmldhfr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3icgluwcc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wgxckdjy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xfdqifzg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ewggnxnd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hnafmzqi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hrkkcyji.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3okuqpvbq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yunrjdeh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3umuayshf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tebahneb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3eayghldd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3iolepayn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3exrbmjfw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fvnsedbd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3iyphtype.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dypbmbwd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fvpyphdh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rzyxgrru.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fjnnmnmh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3texdmbwj.html


<!-- 参考信息 -->