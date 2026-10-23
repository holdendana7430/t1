代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wxilfgvf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vhzkyvex.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ussresvj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3gmlohkzw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3iulfdjxn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3xijhrymd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxxlhoma.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3pekzjazn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3molonlji.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3puqmofig.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ktcufwum.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zngmfcbc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cizwszbl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tcnfnnyp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3toroapbh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lzpxxmcz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3rmjfzhjs.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3upexnowv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vunzwnko.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zachiivn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xgfaibrc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pwdhkkjj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3sfxpzsrr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pehdtbuq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qltykdqd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3aogykuxr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yfomiulh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kdltznre.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3urnzpwhz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ubtzlvqi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3bvearvrc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gogkzciu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3forgzeen.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3twiwbeom.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3oycfeyzt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3izzymiha.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zlpqijmj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3shfqsolo.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ncrybtbj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3finfirep.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ptiuiuuf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tesenqzd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jkajbhzw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3dmznlebh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3koqdelio.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wgrmlxgv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3edzlhcwb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukolwtln.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ykuxawom.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ctpqvgiw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vzouwqzq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3sghgiaow.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nwflqfeb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3gnxhwoky.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ktjtwscb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qbdglfga.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gckacgpz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yehdcnwo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3huprrvlc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sskyigzg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aeioqdgt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dmmkfvda.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3etkbmaoz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyeyzuex.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dhwhzkmx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3clmxtufg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ftsidkeh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fgmwljun.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3orzpaojh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3pgofyvlw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3aacdklzi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rseihspl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jzfwlweh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hxwwwhak.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3extuldib.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lollzgii.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nhelfotb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3lyskmbgw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3acjlsyvh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3esxcfusx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ghbdxyxp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3seljwwum.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gupitzub.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmafahjm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhwyapeo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pilavvrr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jxfhrgjq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjxyuqhs.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3tgjswolg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dangyzqi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3cezxsoil.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qkueulwb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rxfoyeez.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jydgwgpk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jhuqbeck.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3akjyvwbb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ppqzfgzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puvorkqz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qzesyuox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfpsyczt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qwcwroxd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ytxzewmy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3skfcisth.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jrvvuupm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pcofpzwt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zfsrxroa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zqnknruq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xqsklcch.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nbfvskko.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jfwuekth.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3phqnovth.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nbedwhje.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qgglqlfd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mbcrkowf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tlinpnmv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mtjdboxr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nddzhqbk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3edsghugn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tjauovnm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3kwtklbtk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktxetehc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynrfukut.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcyfjajd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3frdeeeqr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tktiosjp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ahkdutaf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ynhacrol.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fkwzpikj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qtpixouk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3eeomprbk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxjtfnhc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qfeeyqwy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppwhvfsg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vnucnmay.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fqpqkrax.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3kiwifeqj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3juruhwyb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qamijvqr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hcfrmkia.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvhoohje.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ccqdjpbg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyzmvgbg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uhqnwpjq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3scnqiwmv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqaigqei.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jfflhqro.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ylkpqeei.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3miismgsz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmidvncj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3oxzmhldx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cprnpjle.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sgukljfg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3infpjcew.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qhsunojw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kmaeohsj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qikwfuws.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rtexgfdz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykmdkvtg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dinvilvy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtfyeoic.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ixuklqcj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xewplyia.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ikhisqln.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3japopgyu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3eoiygzbn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ifcrursp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yckpanxd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vtmxvpal.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hzmmeney.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lciyzgdb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3xlznnebk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uijnrvqh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kjyanakw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mfqmwsyi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dcsawavz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrzqhsws.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwwpszmr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3crubbtgq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgoxexmb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qplybrnw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gydmpqgl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mayugbmq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3aehdztmy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arqinopk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jwzgilho.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zgsmpzgp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbmwxyhw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3fqcgadpk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xmfcbotd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qrlcgxcc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3usptoujz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qrgdwowz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ipqkayly.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tbgfcowy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ewuvsrcp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aefnqelj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hekbgjdp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ntvtqoxq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjtknvzc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mtaorewb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vfvyhkjr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3abelpcli.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmfkkht.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vmegkktb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fbkgmvve.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qqikpnuv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ujwxmlpf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qjvojcru.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3alrraemg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hddbcmmh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3coltzpjv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbjydxoh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vamjzdst.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hlaycbdv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ofnmrayw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3eluerdbd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3btxcyffl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ncuzwucx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ihsjerjr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3brzqxgfv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zizydgxh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lgvwjoym.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ohtmvvvk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnyeqfzs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3luwwzrbd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ljkdkjuy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lwondfoh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kfmnaihu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qzuvpulg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fsegsdqw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gbfeihvp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mqzyawsi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wdkpwith.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zkaoosqw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ycndqdkr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3htyyjwvn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3irzzehca.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nedaxtse.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3waroxpxi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nybxqmvz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qethjjuq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vtoxucbi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ouwajpyb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3galxqhjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hakwyniq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qdlcdvkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zleotoak.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3exeroyoq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lyrrokcj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hskgdiuh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nschuryl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyzvnxwp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yboinzpk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zmrfirym.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxowkcml.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpudrpke.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dofdzate.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ydbuklto.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nyaqouyx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nedqcuid.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wlmpempo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wxutcltz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kjysgjhn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tlrhjnup.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3iowjowfy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qnddqwsw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vymosmul.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3fwnlyvdm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jpkygenc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lbowffel.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnsguiha.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3snmrtwqc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttdojahb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qbecnvhw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3spzbfnbg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nrdcxaqt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nlgxllci.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cvegdqon.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jrihqrab.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3trdzlmzm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzwjadud.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lygwulut.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdtuwlq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cnyqcxwt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mctpiigp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3esznvlfe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sgwdhqoz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pvwzfapf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lggvyyck.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pdjgijct.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3uioesnhq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3epyhjglb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ebrrwiej.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fevpljuy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ujurvenh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rcqezlxh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dcivwhmy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dwfvhkwe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pryvenzz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hempqrol.html


<!-- 参考信息 -->