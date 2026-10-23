代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tippeznl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uxdbnkiq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gjidbnwa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3blxmfdah.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dklshiqn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tskddsmb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gklufghu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rqoxqtib.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3chmqmqhp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tjtwhjsp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3fwtnctwk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qupkdalv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3scradlpo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xnatzaww.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksrpugri.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3pburiert.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qrbmroil.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qybyaket.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsslnmpp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3lnosscng.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mqrqexid.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nouowaox.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fozikbvf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pecktfbc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3trzfvshj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gujvifpt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcokdrlr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qwhmgauv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3szcdrema.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mpuqxili.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kleelqly.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3etqolwvb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3evjnkawk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3oakzfxco.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wkkblfub.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ftluecul.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cnlwohuq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hyuoipep.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gtxzohxa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3roykhkoy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jdfjmdii.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kmfjmwfx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3khrfkygo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lystirbt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hmfurxzc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3davatben.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3bosvnvsw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mmgaeper.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mmhncjrn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xfuqcdyb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pzzuxcbz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fsoijeqw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pwpylaqx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qjhwdxau.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ryghvfuu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3kheawrwv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3zpapstwi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3riodvwnj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jyjqiuze.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wbgskwzq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nsqgtqzt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uzhuepvc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xrfmpxvj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3amleasyy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mfpfxudy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tipawgvs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vjlothio.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3udgfzzhs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ykxuypbu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3tqhzrdxd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifkdbdeh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ytbhnshc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lwmvcvka.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bvhvzifc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hllgzsnr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvoebyu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rebdhdbu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ghdtqkqq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pwlkhzdh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyakpvqf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tkevlabd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tnoqztkh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3nodivsbp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3bjcxtyjh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mvmoqwvv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3guevhqzq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3modxnijq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3dajrdmaw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3enirqpqz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3yzfpdwtc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mzbtkppe.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jhqfyidg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kpjtkrsn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ntxitzrt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3itxvrxej.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3aibsrokj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwpwbivq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xhjojsih.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gufsrpnh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qovkgqxu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3yucxlasq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mhocgvzf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ytacqqfr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qzxvnhve.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3usbomjjx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ubqdmcsj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahuuhnub.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3iyqfeipb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3uyqdypjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uokespmg.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qyxkgbww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efwqwwtn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3tzpfvabu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pauetzol.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3amlxpsym.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sziwuqgs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gqamppzo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rvrspprw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3jiqwplfh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3zrxmcadf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vgqstshu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hcashukc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3buqgmtug.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zyiuygby.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ytvynaui.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgrhmd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3olkoxkjw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3mghdrhrj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zrdnafqs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ucstanhk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kesnnkbd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fvtsvyvr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bimlmtav.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kicibkoc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mneegtlk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3duolqzgd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zvyxlxmg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jaikelha.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uujxdugv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ptjgobye.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vyteflsc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qnxwfdgj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcpkkoqp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3stnysoea.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3geqdmaga.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ictztjsd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mlcglmau.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3syupvdpt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3olpcblbs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dlnizbkv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vgriayog.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jerwmmym.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gmosxcdx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndkziaxd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ejkcyssc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3demkutws.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3etywsjsa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bwtrrsgb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wapmbptv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3gwvkgfdy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qkgatrnv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnuxfprk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dfnuuchh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ecjfcvpc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3laewsovk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjvcohr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vtymlifu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vehetozf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3tzwgopqp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3epbelxkm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wepdrcwx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3boahppgr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3caeeehvt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3elvbawlp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3halriixl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yxoovxhy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xkagxzqt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vphdqyvr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zbqthmsi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wxxxeosq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ytirpvek.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tgdwevsr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jalcgbiq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vixcvpsn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xahsvkrk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ygbnufan.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wawtyafe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nfnmmibo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3arlmcsja.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zmqhlgbc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3beffbomf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkssssyr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqltyfto.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vvfsvthm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tsyzjfoo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlnovwol.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zuikgzvc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gzzqptrg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3atqkihig.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hsmwyzpq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kuggmgvd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdrbhjyk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eqigbsyj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3byrdhhyc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hfqejlgw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3smtjhrey.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kwxaacnb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3btkfrmdl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3elzikzbc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oefjqvps.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qzbaehpt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zklqaoob.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xfwpscjd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dbemnvdl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nwuadjyo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3suffaehm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjldeylw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3naqfiuqi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3scvbvznh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dbamcfvk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pzltzumn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ogejhhcv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ohrdxfaj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqkwmrfl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ufikqxng.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bneganto.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ddwjwmsj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dzjotooq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mqjxcqia.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rhflfzku.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pifrvvck.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fjuotlpy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3antinzel.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkfndute.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shmpyzpk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3iropmnxo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3plmxpxiw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qmjzpkjc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tzdtjhni.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3husvqswg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kkgcgtmt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fuvhrwzp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ppxmlxua.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vciafyjv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dazjjkzw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wsygnqld.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ecbuygtx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qzxbzuht.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jmwjamfv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3uidjcuim.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hbscpljv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gjxwrwgp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ntnvoymz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3sbwworpm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ovmxsiyp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hwumzxea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bistcgyl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vvmdpfvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bduuwbjs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3moddcdmi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wftqnchi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3efdamete.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqqhqztl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hdfbgbwx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wgiscdwf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bvseinwr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jzkbgdnh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vkrjfftp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3udbrnpqg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vdovyoep.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3patlhhyi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oedbhwac.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wttfriyx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dstnvamy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vnylihjg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zchjamwy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bxfrzgbt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bwkkuvhj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nvtyvxsq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfbyubug.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsimvvvv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nofwjxmo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iehkcukb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qgaufnwg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3emlzhdvi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pcncihhn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dexkuemp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3oedclagk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ctkgmooh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ifizomwk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3apftpslu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pjxilpyt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3izhbafwx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tkzsfjhf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3abwocwam.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3yvzrsmqm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uzklyyrq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qhtbuktw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wysereyg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rmiupdml.html


<!-- 参考信息 -->