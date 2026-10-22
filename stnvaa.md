代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2hanwyzyx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ffosjmei.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ghofdyyg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynxaxoqv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uhkrqoph.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qpygqtcq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzivbjsl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dhtbokys.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gddmamrt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xkimfryn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2doutzfoq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uqslcmgz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qhbogszb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqwiepes.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hzhwahvs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vgiupogo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rhtwhwty.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2poblzjgb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mofemqam.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ellubsoe.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bqgdyfho.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2iqfvknne.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2yjsiokxh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2zlcqprlc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2aymjengd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ocwljzsw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nvijwbxt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2tazvyzcs.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xaqiacvu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tptppsbs.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zptfqszv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wjemkmjo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2djdwzpkk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fgalofbg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2pfipmckk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2nagnxdgd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2gapdteyz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vnecbmos.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2rxnmhwrn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nwhlkiab.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2yfphdnsl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2klmosxzl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2inipbkaq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ofzaqgyd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mzwgdzpe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2escdkbtp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bgmuaynj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jznvetjs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gsotvqut.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tncrllvq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2skxsvrzo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2niuacmgx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rrqgbxlx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2igcnclgs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ajkrlspt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2yldljymb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qoemjlpc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2txgfmkbe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2clixqife.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xzajdjoj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fqgypfdn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ueonzczx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hwtvjrcr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gafhsejo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pddzpnty.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ijosqfjs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bffmroia.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2urecdrre.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2eluevule.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zqajaaiv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jpukshah.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2uoxhvzmp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2btirtjur.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ywrpvzuy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yuojddnb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ovozyqty.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldjkwvkf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wgekkrxh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cbpgiefc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ydhuhttd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2fkkkvzmx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2eyyivhfb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mndvacxn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjxxntka.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2dsegloqu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lkaxmnhu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2igqwfmro.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gicglxvi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2rpzuspgq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hpkbetkp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2andpqrbv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hidrttmn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2puqwdsic.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkzxujr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2znhgixjf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cdqagcdt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sjxfmkxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjurnibv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jqwdcgan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfqovwvm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yfuwfhdt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mitsukyg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbjscwhn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zuqlpqcd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sirqdmfa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2worrjsoq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ioqgyuep.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tamqvonz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2loltaraq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kgnrrmmp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uizakrmu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeqowopf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jeusqevx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nvizyjlp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vczexcfk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2annojndu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dxwdzxvj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ccyedssl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vihacpkc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2czqfkcsa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2odwkrdjt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuwwvpsh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dakdxmdn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uabzqdmt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fhqrvqzm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ucztmcwo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2puygbghb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2klkiyvyb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wzrvyqia.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsedttyv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nhbsulay.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hootwnbe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryeaasmq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jvlrllvy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2trznlyeu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgtzaddp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2djapvpod.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wfgwawln.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgipdjjq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyofuvkt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2iujmpkhe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2klrjucss.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zdvjfhqa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bigyqcqa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rymohffu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cppkhoyf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dsfvlzds.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kpobytnl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkmfidr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzqlatvs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fljrzmnq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2aqsgdmwi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2smoffsxd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2aplthjoc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ekuszljp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kknnvadb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnzbnsvt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uybmcvxk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2isobjwxb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jufbvowy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vvbdhlfa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yaqyxqvb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmpoirby.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mvprzskt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2sxfdzziu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xmvoutkx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2llbstznb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2naomefyt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oehyzfwp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2plkwfblf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ymgfisyi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cmidsnzv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tsfguczk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gtpktetl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lxmdrzuu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpwzylnv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qesrwejv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2raknfekw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cvkjyosi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2spjwsonf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zmnjirvq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2nrlrshix.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zoefazhs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2dfjqfoun.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bsmlydwl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fksyctvq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mhlajnvx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tsbnhceh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2yesynvtr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ohzxgiiq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rishkrch.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2censfwiq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjopbiey.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gdevebdy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fjgsunzt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rfiivojp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gtxlqlgp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ajvpldmm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2eyrcljeh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2saelgeyk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ypqjwhea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2erbpldlg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ppmifudn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qvnzjcln.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dpapaejr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hpitnxnp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2aotadtsj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2noiwjpis.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tnyikdsd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mrffgovj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ydttmukl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zuworpwy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iosdqevw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nyfppvtj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ecvxgvwu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pccundxq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yfxnfagf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tojxhtfq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rboqmidj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nfudxywn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wrdafunj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2roxjhjqy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xsysuyuy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2maxlwexe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cpvmbihq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kwuppyhy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hptbmodi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rrsqknlm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zpjrehbe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lyymtkne.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gmlcwbfk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xmquxkdw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qufavrfo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wagtsbfg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nqwwccui.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ktztwggh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2unjyhblc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtrwlbao.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qlsawwlq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vtgwutel.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fhhgnibu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rwdypijc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2imegetxs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eoocqobw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfnqbjjd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2vujmxtda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqmfodpe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oalrbjdb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2potnbqmg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hxgdjpgg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnshxgrs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhdxuihv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuzizuzu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vsfhowsz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wvdrgdnv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2behzfksm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ibhrdmkr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2okewpzku.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdxwyi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jqmxwwvy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gpplzrfu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2wwvluije.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypeasxja.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yqkkppqx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ulkdrdrk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhkskdcg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bgamorww.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2enwpyhgz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ykxkvlpn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvfdthvv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnwdtjua.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ueoizvye.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2adyfyenn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2kpislqxd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2oleqrqzj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qbhsopdv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hehijkpb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2keacleay.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2neujbiod.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fcrjaztf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2njlfwewq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dojrxbfr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xmikqdip.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qhbtpdhf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lslntwgh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2hwxppuqc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hoklgcwi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2owveptlg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pfhqjrni.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvtfmp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wsvywern.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ovjtuwri.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pugpvetw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2psngastl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tmfoqddv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2timolbvz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ybsrmdch.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ezuedbkv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2iqvgwdkx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rellmzfg.html


<!-- 参考信息 -->