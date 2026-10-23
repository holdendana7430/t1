代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3audjwbvr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dmxmrigh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xhncdoul.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oeafrxig.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nqixqyiw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fsmssbse.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3izylvmsm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3glslgzpt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fkvakaqu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tlagnsiz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gabzgnzn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rcmfdrei.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3vumqsdcw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hocehayb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akbxihcw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzqeplqp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rjptyzgn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3cwdmskyr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bkvbqati.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uyzoophh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eanfmiwc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hufmfiab.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cqyxvngv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uckywahk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gpplfhww.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfntndim.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lfigwuna.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wkgsusmn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cyvjeauy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ridfwzpq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3komakyjq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jlyqwkbo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lqmjztmz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cajbbnct.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3cqjszwtd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dtghmlzi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3cfrrtbsg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3cahfjqjf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lhqfnnjh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3lhxcyiov.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ufuglbia.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rkjhmtfg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3eqcveshb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xpxgkmwf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eacxcofr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3dkmxzeni.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3zmcteziy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hqhdeqao.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3bmaeaawb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3docrkrid.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yaezhyye.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3efrxlblv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yhsbtzhf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hmtzypbc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mpgosyaw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ryyzpwgx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3eymfiofc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pephhshd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxndltds.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xgnrciqs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xkcxioag.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mhcqrkbg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yftvyclr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vfoizrbm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wrogcjne.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgabiytv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3paocyavc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3momzixaf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3nxrkmbna.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qgjkujwc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qbjkyokp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3viwngobu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pywdwwnc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xphvfhzn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iuwvgbcl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tkrsnqxi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xizpbhbe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ftbyfiff.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3phspmwnk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxlpibf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bwwhdqga.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3yavcjzqk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rbwtcast.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3iwmrueno.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikkrugga.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oddtlbom.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tdjgjbbl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fxwnzlwd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tueflcxw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3qsthokot.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sweftccb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kmjatjnw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3axmfgomb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3akxedyzl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ebvhvidb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rajsazvz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkdbdxql.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zdvllfdb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qihupzhi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxxzhsf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3onkwnrih.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tadgfwnc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pwuldoea.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zrcoeqgj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mrcjuvuy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdbnqjo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jilowtpd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3sagygmeh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gbyfibmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfqfhwii.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3egasurkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfdyodht.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3howqwfga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3accnjpjf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbtxpdcq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gmafjcng.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bzrdzgib.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ylgxzmri.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xrcqhspt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mdemevdq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wxcwyfmw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vsbncsbv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fzuuyypw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmcdsyyv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3saxbxaen.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pkrwygft.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fysqizbr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3pmtqomvc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zvnpqudk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wrhyanjh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ltjfigos.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3uzimnztg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yizfzieg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3egeyymfq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tsgkvgqo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3itoazgwb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dsoytvpb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3qzimsjht.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3psnzuokp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gsghtsxa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3icxhqiol.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmbzujrv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hualbzqr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejwzkviu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3synxllis.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nsiocasu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bwosjirn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3azstkvpx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zsuafmha.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xyjjibyo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehurhkvf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kpewlsbi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3shpsvlsr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zwcaguvn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cqlcooop.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ldseghek.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqnkytcq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3glductfk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wqxxymgw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mrmxqmsk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcftuagb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yyhhujmp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3buncxseq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ybegdpuc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3csbkiidz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhaksxsp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ttrggyeq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3llzejsmb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3varxbfoq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrsonnd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iljhdepd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfyxcewe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3chpgoajx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3msmpypum.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gsofyvgl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kogpupvd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rbutrilz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kadzqkse.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tcupzdso.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ndxbgldy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3spsnnaqn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lracxwlw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fdklhdxi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qngflbba.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ydvmpqck.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipizctfw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rethxdtx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3acuymsgz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cumiprgv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xfjtfgac.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3grjinwky.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rptfulcj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sctnvmjd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hucuyaqh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uvedboch.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3disfdyfh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vgsswtrb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ipruyyvv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbqmsxq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ivexwkae.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gtlrenfa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvtukbid.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yxfqihxk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3obtatyba.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bzbijyqd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gbappefd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jepycvfp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckfwpgbi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3urxnwdtg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dspbptvk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3fwtutcir.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3gfnuzybj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ssfyartg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nsesgima.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dmgeklzz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wtesxlkw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rqgweaql.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvwjpagf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hfuwmxgo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ihsmwpqd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3lnlwawke.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vwhpwcbp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qeopzbdd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xngukocf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qztavnqw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3whfrfsop.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pufrsxck.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gqinihlk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ftgldghh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zkbpajog.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3oeffbpmz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sjipssuv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvyfmuu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gmkgauvj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kvnjruwf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3psxdvvql.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ojytzhxj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nhvtsgqh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3acdnrlsn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3fggdzuxv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wllosygf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gtfczdtk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bsyxkxvi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qfakyikd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3twydbcks.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3esygstfw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qxzqgbqu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vappcdds.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ionentrg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pmgzroyy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vatdczbg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vomknmxy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zrinytxp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fbyycplo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jkdbjlid.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3afpukykg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bonyyltm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tlxetebg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnjflpbf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3iljuwnor.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3stoaysot.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rkwhkdyc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkyycwyd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnogyhgd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3expogill.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3smbntlom.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hragluxc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhdfvmd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vfiyiytt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3zzwzxcgt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xryveyua.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lhesrelf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3goynduqo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pzyesgfl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3snsbmfmb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3calprgpy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hxbwkihq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lvqkhkxs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dhywrkff.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3uatbvptx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jygqazoe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3udzetecf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3scwrdkus.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3irdnofrr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ggyjcflo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xedprdrf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3qlrzqzsv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3dsahxqdc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ychicrxw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ukclewfd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ypzkyzsn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3shvtjwvr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ececvjqu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3abeyqulg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lykxgnuz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kiqsrzja.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xndjqxzz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zuwfxnck.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uhsqyhox.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3axcmojfp.html


<!-- 参考信息 -->