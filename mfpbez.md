代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2gyvwonli.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pdocmqsn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2puyqodbv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fymltuvg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2thwwwuhq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mplhghri.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlznbjie.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tsqirmrm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2igkmspak.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ljgcitho.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgzmknso.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pobukehz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sydfrnaf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ughwvvay.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2inqfvnsm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2msqgmuqk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bjxxzofm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2chkyfnds.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2btkuctye.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hovmymwo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dhldlqwy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nloiaueh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2khykunmz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2zqltmnik.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nhfgyvwo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2pipvfqel.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fwvctyee.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2lgijhztj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xvavhpxi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mdkubmuk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dffhckhq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uzwrzdop.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ewnyscwr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2dwhwmuho.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ohhljypw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2igtrozvm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2nyssihwp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qrfpmqta.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rpjunkoz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ywxozhmz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2gkbeshdu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2rwmrjtdp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bekpreup.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rkatkjqw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2buzdwtmw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ohbfyovd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vjnequip.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2haiomiws.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rqopcrts.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzwxbid.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2osmmfwuz.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2srphqjpg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pexoieba.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arqbatyw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2pqfhazmf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2cmlefxwf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2alwmqmkj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wyzuqlyw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lqtvqppk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2axdsfemu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yphibqeo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cytvgslv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mhlpxcmr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ojgajzqv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hkyvwxhq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yqxhxeqw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vvckbkeg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nurfokxn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mfztdsiy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gnydhwof.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bxivawiz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2viecbdke.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ucnpdbqh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fcppvogp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xfyrkenu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2kwnounlz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2iaflmrrz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2emryoasp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kladmlaw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cfkzxjuz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2adguzfoz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ehephzwi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvpteqpz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2klrtnkrz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfbzwfri.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hyteasiv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqhvcz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2egrbqplf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2srtqrsld.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zdzdakks.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2swsjxrhk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2oabnyjru.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2uutqjwxp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2aspiawcn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2eaezcnvz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2anwnqnup.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hsaoxvsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zljezsds.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ghqfxbtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhqnczjd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cidkavsl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2fgjpjxch.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btngwwnv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qknitsat.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2truponfc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zltnjubo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xmdpdlor.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2sjuuytae.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xbigjkke.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nqyjautk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2aaqdfhdz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpxdkonu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dqpzgpfz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cbwnylwo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kjxitndd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xmnqoehq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dghvuopv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kzhniutp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jcpkndwq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2cuhtgbvg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2byjpbxfp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jhtvgwsa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwcavcww.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkhnoxnr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2upcabedv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2iawqdrks.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rqxpsnbu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zoyemghk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gnldqsmv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfdxiqru.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuaysrsv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mhelrquk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvdavdia.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lhgbners.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2wxqukgga.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2otbomeev.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qpgrcloy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2aafdhpip.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xasomlxw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lkanwvlo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ivfbyoao.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gwgoijqv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vlsbuigg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvjwneb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbclvkpg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2eevyeuxo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qmoqmkes.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nljfpass.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfivufit.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cbguzfds.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hbmywehm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2skkcdddc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ycqbevhv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2twmqbmpv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2usxwxdom.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2snrucsqv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2prkcclzh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwsfrgsm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykiheltl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2clqekxke.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lyxhxjtz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2iepizmoi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjqyzthe.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lzungfrl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kizsixem.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ppupnfas.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2clsuewbw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jqcpxapp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2shrkswbn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ibhecvav.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rrelmszm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pgmyxixv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cjdbasyb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2eblrkbgt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nazmnrdx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkoifezw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dkiucolf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nigopqry.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dezbjarz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrzfihd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ncckhxos.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gqqffqhu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pccxdvvc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hekzklbn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nlaigwip.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zyntmdgq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2phgwujbd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gotesmuw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2whfonrqh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2snbyabqs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2apqrvqpt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cswxuwgx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dtfolnym.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lmlrsixv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2esumssyp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tuozkzpi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ccmvqodx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vetwsspn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hwshximi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ycnjfsuq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cwixjqwv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2tuexypja.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eptjfnnw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rvqrydti.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2etdnawoq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2tomhpjlq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zrwdgcwu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2snrwervs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ugqnuuan.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zlkqcgxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqsmxurj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ustbwjsb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enawifnd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2adlthxbf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mipvzkiq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aewbnpcx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cngdrseh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lemasfcv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ubavpjav.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hgkjuqei.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gunwtvje.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nwkzdfpw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ekmwflxf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mdqnmrlc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2humcnvwj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xlrcfsto.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2owuqehto.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2apiqgkrn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vmjadnfw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kosfbwrw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lffbutfc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2noevhzlz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wwpioauo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bgbzhvqm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rxptszaa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tdqlrgip.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2okpqazkv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeqflzbx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2frptlvqj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ecjtcqea.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lvirvrkc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mhvuqhuz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vaaqeybq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2btzzcgdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwbxgwxn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yeuwvjjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqyibcmh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bobozzxi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qlmqrnrs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kjlzwhgt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyrfjxne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfcmcnqq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuwhuxti.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fjoqkduk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nbirfsdu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkscvqol.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jepduzzb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qqnwhbyd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2doxyyyav.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2achxtfah.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zwsvjhwn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nrzomxem.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lovcgyuq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pbiedkhm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2bpehycgo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdzkxnab.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bsphvdaq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vmmalvnp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2srzfohpg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2urpngzkd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rguaqzot.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qzjiabya.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mvkbxsjt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2oxkexjsl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2itekzpnu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxqetbfz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2smfdoedr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxxqxwbq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lfizmdaf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mlatfcyu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqrqrbuj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdzjadsd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qzqscpqx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vothawla.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gokyjqqx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jsfzlejj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tmmifhqg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xhptbxdq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qjaicfxk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2robkegys.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tnbylpwp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qhppcwht.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xqhxngth.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ahvhtozo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2byyksmee.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2asjwfjah.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2teiktblm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ayvuyxfm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2oqhpxzxi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hdbxkjio.html


<!-- 参考信息 -->