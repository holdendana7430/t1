代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dqgzqfbx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xbkmboux.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dxfgdnhy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vvwwiidp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dzcfqmbr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tdjjwohb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3npdxyuqn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ngxahknh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3plzjpjcp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhgcjzqi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynbrhixj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldisxnhh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wdtpamvd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yfquspqh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3idceecwl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3orvjruml.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wwtzlbhl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ntybfriq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3achywwbq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3omcwgspf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cajzuajb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qjpblazv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3bnwjjate.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kstwimoy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3dxhikzfn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxgpzawl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rvityclk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3sjenbvce.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nihptmjv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pqitfhcy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3cezjzclx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fdjwphyy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wkjavzbn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3wqnuksxp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3sibejcfj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tegvejnz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rozcvuoa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dnjlxzal.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yleucavm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3mjcdspaf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vshhpako.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3acimjwbz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3lpizlpzl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rtfaweqp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3qyjoqjom.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bbeoarbc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3htereynw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzassblm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lptuvuyp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uqvhdntw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3elolrfls.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3icrhznig.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zccgkywe.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3mbvtpjbz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3eaaksmct.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3tcfeichb.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qsfladho.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bhtcubkw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3nvknzrmk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3okufhvqe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bitzchhv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bmxrbymo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ezcyhfew.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbirurdr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sqrveazw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pjyaelgg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rncfeqrs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqiwcrie.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mgorvnba.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rgymkudx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3okqkllgu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3dmoeplcr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3gbasecus.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3anfrbfim.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iubruvjc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3iodoxvae.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mmdrhlyo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gxcfnfow.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zsezgbmt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wnsxtoko.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3qhnjvtnh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhrmwdnl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3msxwfhup.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oilqpkqq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dimziqcs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzskcusr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ujwnfjsr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgsilktz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wahdlevg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nnhcgohh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ammjaqcz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3rrjserpl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hcuudyif.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dmqyhqyg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3akedlexy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3plzhaqka.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jnlqhxpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdobutci.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fyllvyzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdjshbmv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3wmdkjhtw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wzuddvgq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvcrzbow.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vadmmcmr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bwnaaqqs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3spwekwuz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vjcskcll.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wldxokcw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zfjritwc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jjyjysce.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lhzuvstt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3reebzeuz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pjgjendi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gtbcuwcq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eihqfccu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jphzlqzn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3oozehkxb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jasoiqlp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wauvtais.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ppjfidof.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cxzvebfa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkerikvc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xptvlels.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dccbpbpc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gecknmft.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rfltgzoc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fapntrjz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qauwptki.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vlknpbum.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmseiezh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3artlgoad.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lvhnaleu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vycpbonb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3roxkamzj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pnucxlwe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oacorxzi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fvetvnkj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ugtfdqwe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wligcaft.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rrrtlamt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aygiausv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhakszzm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3skwyrvzm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gajxilpx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yszognfg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mqbzlmfi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3moxjlgmo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lahjolmm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3btyijsda.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjivlckw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3djhjxiwl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3uribejjj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vauoqvzw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfwlbivh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3txbxfupd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3unomnriq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qwtwgvqy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nfessgkv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tqyniwdh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fvwtpqaf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vrzbxbpg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghwawyys.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pbvfpdrj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yhveovfc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ouhymlds.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aonvwowu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3waswoblk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xwjrmfob.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ympkzmly.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qfkwtfna.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3taqrtpps.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wfwypday.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vhtdvnfb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3rxfcbmky.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xdawkrei.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqhmrwug.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3valeuhiu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwahfzuz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ffnkuspv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3trjjubji.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpbthadb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dhhnxvrk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hpktsdpf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fsqomxik.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tqmdcenl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xgspvtce.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmrbvgco.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nprcidxc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxhoagkb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nysfmgrl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qlepqrzn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ldqfgzhw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tjgysjiv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3stlajvwy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3geaeszrz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyyrnfcz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zgccovjj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mvexziba.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzazoqqd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pqdzsjdm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lgroiwka.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3czailjha.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ntbkfafc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3waqzerwd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bafsosxl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcsbfjrj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dbuqioce.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3psrbazcr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cblvxlrz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ejqxtnje.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3sitcfnco.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vtcmjeer.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lffgsxje.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3amuimwtf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3guwkbwit.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uwctafjw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fbqpoxem.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3pytvrbdo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3jlffgyax.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lkrczxde.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kppqdnsn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jwdcnngk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xuvfabee.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nucrtgnq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qyjmlnae.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vqhdrqnb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3riedmion.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yfoebgio.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3izipykwa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lzovjfoi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bkfasdma.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dspjrsno.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tijxbnbc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sgpeoces.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ibkvkpuy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ztwjlqxj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bnzpvpar.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nfnywwty.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aputmqej.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pzcrijzd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gumamwxh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oxwdplys.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ieewimpd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pbscddhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbrnkbqj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jmaakbbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxayfeuy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mckppqvb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3iizwifny.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzafexik.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aczwrtnn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3heznapan.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qleriyqj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ikdfjnnv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqmpchmk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3flxqkurp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bmjhdrov.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ovbiqucd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3evjffpsi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcgsiszo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dxcfftlz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3eqariyfm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3iyswdyel.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jlwsritf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pgegsppf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kguyyrni.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jawblqei.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gmhnayiw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3iklgduyd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mqhyrwzy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmfgbspb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ehbckwgx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dfokuoff.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rhdsejwl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3izpawdbr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mpebcasm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3cxcpmfnv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edfbrfbe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3iqhvwzpu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vueizwna.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zepgfvzh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eukaeqmu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3swctunfr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kyqhekkp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cbiilhgj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3cgjrdhqo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3njdxmves.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3drvrkimc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zrclknel.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fpczveli.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bwsodysi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kgrfmtki.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lulwegxt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gdendblu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jlygzhrm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ztsxktqr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qzpowgpd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cxffiarq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3xtegymlj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3stmrccku.html


<!-- 参考信息 -->