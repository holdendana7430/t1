代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rxrlqpaa.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3srfobwjk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbgikqda.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3reclwivi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gvidtfsj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zvyrqsyn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xuifdfqp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rkiubpfw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqdwyxif.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdpfrbyc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3juanxjez.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xtkyayte.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jayjsplp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tebnshyg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fxjrvxxv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3osonjifu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cbdxsngx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cttyhzvs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3nwxjhdpw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wiysawbe.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gskewuht.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jpjxajun.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ibjgwvqv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mtwrpwri.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3azzmkmsi.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ueqxheib.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3peebrjgk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3quieomdr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dpeagnuk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3tbjuunuv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mqtklnlm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3prptgioy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3chjmvtks.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xhdenipw.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3evudougv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jixkumuf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3selkpusj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tppjibcz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3gsnvxhmc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3slfkeeqb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtshdqbw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxexefd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxdazzfa.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mxdppmfb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xuamvxcs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qbuzhbdp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xtkmedqg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3htqorvdl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jjjuotld.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlesnwxt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3cuopdmre.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ehjnsvkl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ksokmnvr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zueqjnhu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3ibsolfft.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3moezczle.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mhnojiwe.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zpkjbyyx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ymfybpby.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbcbiafp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ugwpwwrl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jykcommi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fnlbvcvv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dhkjeseb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3znhwoees.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3culzqnom.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xlirnlmr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3szygtyos.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahwngtje.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bzapgrvt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3usjezhog.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ccuwnpsq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tcnguqkc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ehchshbq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rxiviewy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kjpihwmy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cpnhacon.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3xssmzfbj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hodlrrke.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxzztaz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3fckcyedj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3phwkrzjg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3cgvtnayn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfjhlfx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gxtjdumy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xknrvpkj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3akejjmxu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uxspecds.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3jdlgzmmp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3htnvnyuv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3awedjlnl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mhwccyqd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zxzyvknh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3selqyywy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nucotdei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyfrolfd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3okomvjzp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fblxwhlf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3omxhrazk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fifjlbtv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xewnjjnz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hjbimvcm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qjymdsve.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3iudpuxcl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eibryubt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3acqejvdt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3mqdwadrp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrnnsgew.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3frjxdmvo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yjukqvck.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cclgjeca.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qzexapia.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mzmiaaxf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gncerlfu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jiurrnjs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3virqmgls.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fppqhknj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kasszcty.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zvggmutd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3galqfztx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3irrjupks.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3mosypxxp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hspvbpou.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pyuenbsj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3apgiwxzi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkxmbqqx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3azjabszb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cuceeitv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeorjgjd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvdqxgdb.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3skiegcld.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3qgtcczis.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fdyqlpfv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gmhppaze.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xabtigix.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dftdxksn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3shyjqhtv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxttulbx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3evszailx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kwxbbokt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjhkduqx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mfsomhal.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3yafstjpo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3nbocxhxq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jblgaxvf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwoggefb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3psuwwkrn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbvqsgo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gykhfpqj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3crozfkjh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qtvtcwqv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cngfvqjy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziqkqgoc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rreaggkg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjpeswzu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3foillgwr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dxpnqvvr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3owuolvlz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qyhvkwww.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ypwrfklz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uttsegqg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vhnknbmj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nlvtpuot.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sfgkqmae.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xfefyeds.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mysojtnd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tjekqlav.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cotxdyaw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3mvyzrcop.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pgrwwydr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ivcvlsno.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mvtmrabe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqjjxang.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecuvxpyo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yrzhoncg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ynsvlecy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxzgbxvu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wezvctgp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ytpteegl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gtcqzmqd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pkgeefpc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gtjsfvmy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hzmswaib.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pxtqgbvs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3chuhnzwq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gcmiailb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vhuhnwms.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zwultafk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krvlmhxf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kjotjodn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3miwmmshn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcizwoig.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3rtktmhlz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aayxjqrh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wqfsbauz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rhubqtpe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bbbzryqe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dbcxcaof.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tkoswnrg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xobtmnqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bolfhayg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ifuowsuk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lyhissmx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yitgstpa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3emxnpaof.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zoehdsqw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzxoqycb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udzfjzvo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffyhqoco.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3aqatslbl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gdbzmrow.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwnlnvl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3auuhvjah.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ldzbaywl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ctsxhzov.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ywifargo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3brtcxymu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuwuwflm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rsccxbmi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pjofckeb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjiznbzk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frptvdwr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3smpcvyut.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bzvfinjm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hjzfqkux.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uippevtv.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ynnhssim.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tyvgvjfd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pspjkehm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pymsxaug.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eedwizrs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ygnoknei.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kaoonpmi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kigrypeo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rsdysusz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xhqmdsrr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kpylatna.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3clcmjlzd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kesjldcd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wpzfrvkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gopibrbj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cumounwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikkodkht.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cqggockn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yblohkbr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jlimsgjz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pivrohkt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gawqanir.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nspqckyh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wbkinqno.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3sqobnxxi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3krhmnjob.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xhujdcaz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yglfnutu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hdrngkrm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qiblwbtf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wauxtlcp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ghvbsdfn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3xtxonuqa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pjuhcvgy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3srbkpqjs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cbfiukhm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jiywbhoo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsivmrvo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wmaxjdyl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3duzhfxox.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sghnibmj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3cpcdmufx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3skjqlyny.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zlkczzxh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3umodbxpv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dncyxjqy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mwgbblzj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ggelydvz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3iurirdgy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dswxtszn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uguxxigg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3whwbisjz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ekenckkh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3baaachis.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hrdpwtxe.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3taaewywm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ijcvoeqb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3obbclgoz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zaygiqjk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xwxzdnok.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3assfmozl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nwqylmse.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gmsbycdx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gesvdqme.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3freabpem.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tncccjux.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tugfcmga.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ipjgnloi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hufuevot.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3frrhzjbq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3izdlupho.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xmxczlbt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cvbsaxkg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrkalirz.html


<!-- 参考信息 -->