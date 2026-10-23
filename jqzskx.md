代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vgultrnt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gpnrvuyt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3uyilarzb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3uuydrccd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gixmkeec.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kkbdvpfz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3snmtztna.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jqjxxslx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3srgbkwzw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3pjlepekc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3yuawzwjw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3elnjrzgf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wgqtihil.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ratsygio.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jykqlkli.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uenpfftp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fzkvaqem.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgpvqten.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ahxatelm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mznzknfn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pppkqcdb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jxrpjala.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wdzeqqyz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xeqkvvil.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tnqhpysi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfmqjsp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tpkkrsqx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3oerabsom.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3btdgbouj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wqwfkekd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ehpvddxq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ugbatktm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3yresumxz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ecshlhyo.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sepxpwwc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3drjuwvsc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ljsacjvn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xhjtanuj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3giozguht.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rnrsdjee.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3enctcpke.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3phelcgrd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hhgnkjcl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vgiryfiw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3oeuxsfjk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3zbijnsnz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3bofyrtil.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qvfkbxpu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3gojlzktf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3kgifhwip.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wnexppev.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lzczoepz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3lttxlcmt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3edfkewqa.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3flfbuvsz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqehhpql.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gotskoow.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ocaryzgc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ghkrtjse.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3oermxqoj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mmbbwsqr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3oclqtdnj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dcxmfdbx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ehmethgk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3obgsmnkh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3rtqmqejh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qriyvksv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zdnwxuil.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qttcxyje.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ojynsnzi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ejryfwkt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3iliqrrgj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dxredarf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kjkhhoba.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3frxoibrz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3oqulhthd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ohwlzive.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zowplmxn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jgkfknvd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3brgxmyoe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yxptlzag.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nhjjbqgt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mcgfnwij.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jagmgzfm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jlfyjmez.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qlcbtvmm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tvphxaof.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvsnrpin.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ssxvyqag.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hehngjrc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fypshpsi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3egeidhio.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3lqqsqtii.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhvkltw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3rogbrueo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mihugevs.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3owkrpwfb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ofwjrhqy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qbnevntf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ylrxebtc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3fkvkrfzs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ylvdicdk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tvfgnfdx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cafpvubs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yzofwqwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fydgjjxf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3cwpzwucb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixxinjwu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rtjgeapl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nrhrzjaa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dppwxnlo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ekghfukr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cueljnaw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ppysvgmt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qnivhwgv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pmirqyak.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xleknydg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fzecyros.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ehvetcur.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3gwsduwlx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3klxjgrbp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qvlmyfgm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wsohmhtb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lbhbkwjz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3auxndgmo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3djyilzsy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ddtloodl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nlhpdrlw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sarrtzga.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vinndblq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtwnhono.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhlfnavd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3oitggllv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xgmiwqmb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3acntsnto.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lejbcqjt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rqdikbcn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fvkpulnk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kcxgrwgf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbxocddi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnwvuwls.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fynhdbpq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ogndjdcj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3owokqtjq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cojggnvm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zddtyqdg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdzbbjjh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvnbajt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3txmqpuyw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahekzkzh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3etvgydrp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3witwxxfc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lppibols.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ladrjlps.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vswtjtrt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wbgeldac.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fvidqdfu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxxkyowh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqloxydy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3geqqfiip.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cayxdjsr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3afgldzaz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fwkeznvp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ejoehjrl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rromqmef.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xmjrfyno.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gokuojua.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtrmqmu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3dmlkpagt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jzdtlwrk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iddtodih.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ezdyelsx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3omtoxppy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hjwytgzt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3myncswkg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lhdrwbvd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rxdynfxc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aedqqcql.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hwuvdarh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tpjrgxuw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dqrhfvzp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jffzkhub.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3znmcgriz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dinlqtem.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwhgxpvp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqpjquhu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wdgxxnni.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ondautfm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezbkoise.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jgrkvwuz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lxrbtjfz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdzaxsrq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rlasumsc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bnigqmyd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3imqmhfhm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvvnypoy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3fmixbmiq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fzxnwbby.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bctzcfbt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pprhhwsj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3sjnjchdh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bvbsxryr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rcqekwqd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aaoxmagj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nrehhnui.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3guzloogv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yreqfmwq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bjcsxjfv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3rajttqec.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jktafqmr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dbtooqtn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vqaidvlo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tconixnw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hypwbseb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mmjqvkjp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ybxkamjk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zgxymgzz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3sjtuevkt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3jicmpfbi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eqfiuifk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fxlsvcai.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qzddrrfj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pigiyfkk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pwbnqqfz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pozekalm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vzetmezy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mgtunrls.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ialntzzu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wehnufer.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rimkazhi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dybxsesn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xkpyifjg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssekmzwz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3redvpwak.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3splrrqfb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zuymiffn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xdkafcbk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3axudkbiy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lyiykctd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rybwagrd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oxfmdsxk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bxclxwhn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nkhmeovb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pjnyqmwq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cmaoesqv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zifxxprc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yfuiekdu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ioapxwas.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vzwqhkwv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fiybcatr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3sohdgfvb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gsuwigoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxujpvxp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hjrxefzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcmpxgkd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcyugmvi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3adpauouf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yatnrdrr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpgaejqf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3idmuctxo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgnchzje.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3saznmxcr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrehkxrn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tsmiadqy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gumfvnzj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fmscnerj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ioewdvjf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ylsprdqv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ozirckby.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3omwemrmc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqveoizt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qdjylvww.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3eeoajsfb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tcjwfopz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3yyghwnca.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zdyisqjl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cycwjpgf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3imeknpem.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pfvxxahv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lpjnjrej.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jftbhagg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kssufwur.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gitxhqdy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cjpoazko.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3cikugwqz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pvucdxzt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ptxgfimj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3odlvdpwl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkmzxzwz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzolnwoh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cuglfnst.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3enejcajr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hgczhrta.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ftfoyeri.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wahglxug.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yrlbhwhm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3riadgfre.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ideznzrk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ggxdyszj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fglvmjrs.html


<!-- 参考信息 -->