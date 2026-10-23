代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3sfuwovhi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3obbldyoc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rnyskdjx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwlkqrzd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ulddyxmx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3otuvqbip.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdjyjlsg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uwiwkzat.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3abwjdllc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsmpgsob.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zuqrnfiw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zyibwvbi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lpsmlphl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rvueoidp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rlupflzg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fjsdjopv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nqzhzdbk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jgehjxyr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fvbxbeto.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eeixlygm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3tsyezink.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3sqwbheav.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3kloneniq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nvvtcgfa.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qfhulzbl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqmkrcth.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fmzejxfx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xqhebpdc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vtfthfbz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gjcyzfkt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3pmxkgfjc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sdoifjri.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tarkwgpf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vgfkrnru.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lvsiqhue.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3yauakbls.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hlzklcys.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tjhinehh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hizenouh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bkrmgdqq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nkyzvtqy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hojitiob.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ugqmtwpy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3lvxlsnuf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3tbtkufnh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3injlxlbw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjfwqls.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3frcnqxzv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sjldmdwr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kazrhwyk.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wivevyxd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3dhjxghtg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qlzqxkku.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3dkjvmxgs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ntirqsdz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pptyqqpf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3bagaclsm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3slitftat.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdezyuuy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3hmdoeozx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bpnfhwqn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tltqdtpz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zfwypfel.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynywdzhw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mlbkrnth.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ocwgnwit.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfttrh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dcofixrj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gluwdumg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3aptgntxg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wzydppzf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ghatusaw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tvjsbeeg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ngzryvnd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ssvboeqm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3xvzsyuxp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ahlytnog.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lxsqvdkn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hikucjfa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3asfeayxz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uukarsly.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezfzxzfj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mmvjupji.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rwvnbsor.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkzubsob.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zvnuchfy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vflyjemq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aipiwanm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3yjulzwko.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hplafusd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3aarjqarv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ccjdjcck.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3wbjamdzh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qacjkcor.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bdycocwq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3axntqeua.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rtbaphtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iowidkpw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ndzwxdjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btakmrle.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3sqlovzvg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fkydxtmu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhbmyguv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3onfqfslb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gfjqhndz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eirrhcaq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rjwjylgo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oawgggig.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ajxvhojn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ciebruly.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vwwcadgz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhmfhquy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pirntqaz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3omqkdwzm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fjnlrizy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zwiycfsr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qadrqapj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3syuvfjcn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3pkpzuxrv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3hrodphcs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hdisplsl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ocdxwcyk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pztlnkwz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pdwhrglr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zswnflrt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yacdvjwb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zlxcxpqg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mazoozts.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rnensvlm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xkkteqqf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hzvpnocc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ylumlida.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkozhzma.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fxvzwabj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rwrtbboo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hllaokze.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qijiaqlr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wrigygbs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3espolmqy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rukplsmv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kfboznzj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbpsesxk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cxeobltq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3tkiliejt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ikhufqmq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bwmfwlcl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hxlvtdiu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tionjikl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3okpdduch.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bzkjbxhg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3abjwpqyd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3uvmtkexm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ibnjnlfr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpwqbrru.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3anyefjzp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vvwkzvvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3relhccex.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lunoeotp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzefgevo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3romvjcru.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3teytwbog.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ztdtolol.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gssmxrzp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ojnzzomg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3syapzmcw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3huhxnpbw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nnnnbiuk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3irebzoob.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zxlnumts.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3exuppqeh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fmpittbc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ltxomikr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qzryqglt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3rpcklinl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uubpxexq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3orsccnkc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcvlubfl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3omcldtwu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3isczzjqm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jgkcoewa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3juynqezw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jyownmks.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3odvykhuz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgaxqrmj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kbrljhiy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qaqswyqi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ngnzitxm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3akwniqla.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vfgqutnt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkhaahro.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dyysyehh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pfmywfef.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vsygowam.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3etxprvel.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3laqluqkt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lotjjigp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ybdyzdow.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3sakldhmi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xtcyiilb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kggpcodw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hnuucjch.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ezjtgvee.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gwtibvnn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3otsqxpjn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbesbyp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhxbxish.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3aelmjndf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jcwvabpo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wtldyqll.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3lrrqcwkw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tpbznzvv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwrkrnqu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rngzimqu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3puyymusf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qgempgwt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3tusbmktf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kfvlrlub.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zyursfns.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kmbyfjfw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3efofxmjq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3btgzdgrf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3amuazkcj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cgqygdgp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3uoouczez.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzherpzb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3llrmadql.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3axppinfo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3oxbnhdig.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ngezuiav.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rljzzpjq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ozhkhzkr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wskiowpy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ttxxgjjk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3utesidxd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yspaaqqh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qluxquoi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ffwdjfvz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dpbnqald.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mdvvscaw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mlcipuyq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3exxzzybw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3capjfgvd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ujwzsdvv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yaounhgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dudpjxvm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cjhthrps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xeymxwux.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dqrcimvn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3eimajmrq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vzdaseje.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hoiunpwe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3owwewyhi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsjvsmki.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3eerwmeic.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3aabxwnov.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3johpycdq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3odsscdpr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yyhrhjtt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nlpbqptu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irxegeyx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ejzjzzjs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3nolckrhg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ptgcfvym.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lwccfikx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dauerifq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kuehiazz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fwdlkvvw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3eoezoppy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3szlganqa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aquasohv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvqkgjdz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uazvwvno.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tkqtxvty.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hjdpyurn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmyszosb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qromccnq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3maxirqst.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3unvmkinm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pggraoqa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qjanohdo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mqjhlhdp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ygjxywtr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ylazuolz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vtgyiwgs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jbtmdlyf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3znjotgae.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nvtyylos.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3upeytcij.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yajiwdai.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nrgfhyce.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3kgpeprlx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pygcrxxr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3crxtjttc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qplvjwdw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jjqfandh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3twabhrki.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vcvsfyoo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kakjrjej.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bkjdlszh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rvmatpls.html


<!-- 参考信息 -->