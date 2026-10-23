代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3izxcyvbn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3guksqepw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ysvifrww.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzptnnah.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wregtqbh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lmuigwqy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kiswslga.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uwmegtbe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ccpgmcpc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bktaksee.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hoppmpun.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkexscky.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3thnhncrm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3redbwvtd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ezgnudxg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3okeztgyx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wzuvdpwt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezfrkrkt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fuojfczr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nbikdfko.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzmbmiab.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hlatftpo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hnolwtbq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzynkbdw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3dmdbacaf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mcnbutge.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3anhclosf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3siyicemc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hzsihjft.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nbxsyyct.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rhgyuycn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cokkydqs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3maiosbms.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3gnvgmumc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oaeqxcmk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3jlsyelmy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3aezibnce.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xfpvkxvl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rmqwgtmp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pzfagohf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jaydhxuc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3yjpbhaet.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dajoppqd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3iwgywlgv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3fpylumbt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3hxadkhvv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3khlqstla.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3pcytvyvp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jdzeuaii.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3smdiuaug.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3gmdbmvqz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3uixxtnlg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3lgnziyaz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uousxrls.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3triywvmd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kzmsjhhw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tdexvbia.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nqvckbts.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3twmlytey.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hjgdwkov.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ntpkvlxg.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3bobylzrx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ydqretuf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hvkwgcqx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzlbpzmk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3daxskkys.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3hntkdoih.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cdtjopfm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dezqzock.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ylynijnr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gbldnuod.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vibwcbow.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tenekhjs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lodcxqzb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fjtfinvt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ymzwvmav.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3preoumxh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xdcjzdpa.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3suflqaxd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ofctrshm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhfmwypi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3edmpzugw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vnmszouz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ytrxpbmw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqkmsadh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3sqhlwnpg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mppfdysh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qmhbnzyi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dmczwarl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wemkuwuk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vwttzlrv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ndsthahf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qzqsslcw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zmtzpvgp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xzffkteg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxrvdhtz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3loeytnxk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3uhluaivz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3gashcqxk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jgrpjkup.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3jnlygmvz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mxcdhvgf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3terpsyhg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3whsqqdms.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qtaxsmwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdthktkw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tczpmoza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvsjxbpn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ukreohaz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rldwlosa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3qihjpfhx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bppetvfo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rgrtkzyn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xsfofjxb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uiwcnros.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ibowdgan.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3elnczvet.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ehnjjmvm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3eldqdeuc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3azrmhsgy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pajbgeop.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aumkpfzc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3exthlqcd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3saiqitis.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3imvspjfi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cbggbvko.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3lqnxsbiz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bajceeho.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzutwjjs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwgckfnv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3flpvnbez.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhtwjaoc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3diahycsa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ajidujrj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tfabsszx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yrfktpuj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gupxnazr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3oqkfhxio.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejlzvzqc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qjfynagl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kukdrstc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mybexplj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gbtgtqnx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqpxlehu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tthgioah.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3gjrqvmex.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3evsfrlmr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aeopgekc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hdueptyz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kwanjjvw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cijtksvp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vqbxphno.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fykunfmt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wdqlinfh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3htklndgo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejtytjkm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrbosnnt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3okafceed.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3buobcbyj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3omepwqwh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gwyfxnnq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3haueyeqp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3omyacwhw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjntolbc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3bpdlkltx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yzvclffx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gatceelr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rnqrybkn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3uojobhsf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yewleipb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iimhmypa.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rxshlrxh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ytgenvcl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ijycqumw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nzrxllfx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mudxcxzb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lzcypkmj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uvxlggqu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dfbnvxys.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eoasrjpy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lopewbek.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3luqyighs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bztmewuk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ymixmopq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3stcgheee.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fifnknaz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lopjuxdw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vondpkpv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cnfkitlv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mmbvmpij.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jfrbdwlp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3irygxjxq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3noonrmoq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gmcjziyz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cewobkmn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iemluscw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ivdmjofy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kqtrepwq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3iobohuaf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3urhlwxcf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hccivfuv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oojmtjvv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mzxxzjyy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3frrkzazf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ubypdads.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nfyirrrm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zynmmilm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3agbetepb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3znpyuhwp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ofmpukgk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3epqtxhfv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pufkypmc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ssfxnxsi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3zactxgkk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hkbajqda.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wlgpgzsr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yinclglq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3cewyhlto.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3geefklrq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ofkhoqpi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vydjhrij.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3khqcvdgm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3awhkmsnz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3imghzsvw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3eubslrxl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vzyukgit.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yrnevnez.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ogdyqsvw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3brnkukni.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjgzflcj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdbsall.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3amrtykkk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3htcvyzew.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ofmgfzcf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hywbltqf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ycgjfusz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rizpgeob.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wwvhffic.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pvzvlpwp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3onuilxuf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tqpoqgrk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oxxsqhii.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iduocomt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3pbyxiils.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cpzknclt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nfpqkxod.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mcnapkjk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hgelvywy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iftbugcf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3broyfwmz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ypqjbvng.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sevnggpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgwefbwr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ndzbycsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzdzjyky.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqlaadqo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3khvdmreh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkociwtu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfnvlslr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3keyodtfj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rygtsxai.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qrnakghm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzwyhwoy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qytuhfyn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yuxcpjxb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3puealvax.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3voimgncv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuajkbtq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lpdpandh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zhnavtao.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3faivyvlg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3drpnqsjm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qzfgqcuk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wokaxdny.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iqrysqsn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nezrnfre.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dbfhrwdo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3chsylsvs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3utdqdodd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jtmmvzuw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3esdpoodl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mxjpupda.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3spauiqlm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3znpdkohx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3edtbztww.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpnrhyub.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bzfdrzfl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pgivqnzw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bmauovzb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qcujsaui.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jqshwkqd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mrabjnnb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xvmvupgk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fkzqwcfq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jenldqse.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hwpnabtr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kbuzzmkw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eaggxdfm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3goozsttj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sfzbrumx.html


<!-- 参考信息 -->