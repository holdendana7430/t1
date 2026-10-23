代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mswbzemx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vhesfilp.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ybxovtct.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tucbskmv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpdaue.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dlrlllso.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yumsmggr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3elibrdrm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3tjnlffab.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zesgwnkb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jtxtzvgp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lathuqgy.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3coivoblw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bssalovl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ssmgaudu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3rjbgxgob.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ihatrpun.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kbiccrmy.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3znnwgqyx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ypqdxomq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ztgnrszq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lswcvfus.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3woaxwjpv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3icvdovci.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3aegzbfvj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hlhsnaof.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3wmbeiwwf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3esbpinpf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3djxdupql.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ivbmudkj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3begvmhlk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekoijvpt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3kdhnfeqv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lntdihpf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3iciiponn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3onaqefuh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ssnkkqki.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gccawuuy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sinlkhvf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxitauxh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrnskoam.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oljtuiki.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rnxahuhm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxfflrmw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gnazxqfa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3oauhcyye.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqpzbso.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dsgulhjl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jyqqswjf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3yzlxpozz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mnmxyimj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ecgtetvg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mkqbnqoe.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ezqdgapr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hpbxowcb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ivkoycwr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zclcnwdu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vpheboxr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hqcrbtdu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pdvlggot.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3krniwqrz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3wgrbxtod.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3swknacpj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hasokrgx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ejcibfql.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3aszgekyp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3uohsasrv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ibbbjbbo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ullevcwv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wwbtxfjd.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3uavmnnlc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cvcjemer.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynswmalf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fjeuqhtz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lywfholp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iwnagcaa.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gdanowje.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zhjpjaby.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bbrjamkm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kurpedmm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vhtnqptq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3qloloyqt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3fnpcptiv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pkoskalb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pskqdrfj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pypboswd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgiirotz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gplcgluw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wiutixuf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nbjljmsw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3babxknyu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vliqudya.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3yznfjzvc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jdzzllrl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3twfqopgo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gguclgvy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yupxmpuh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rovpylfs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3adzqihrv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ywmwkrwq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3avpgtypm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yrkmxaaa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fbxnhnty.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3nkkaguhw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3szdoykch.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fsojhlra.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fjvbypum.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ekgzrfqu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3bompsrpw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3mticwdby.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mfifhyuc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqjqjabz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwaqalvh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmhxgnw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3irdsgslz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgopmfd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3pcinlzol.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3eovnbakg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rypebdjn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3rsfohilh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3marusioh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ptztkvpt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3iucdbkgk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zvoysqpb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zwejglyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmlqgnfp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tsvqgvho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpikuvuy.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cfpikpyx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tskhpivl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3forsqhug.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ysmuskbe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ofinkeer.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nqprchwe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3kiklycyh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3roghoycs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ulaqiaqe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3udhlbvmi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dlbxrtwy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpobhdsq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hhdmahab.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tsoqixbg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sitrdzjm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3kcukjkki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3bsglclsv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mfuwrmmd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xwlwjduy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3egotpvmv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjqjnnnm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qkshopwn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rxlncnqo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oytevkwu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3snevsffb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uqyxyfns.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rwgofxax.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dzgfukny.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mdknhnwa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ktvhdget.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbaztrv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xpwvrrdm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rqvfmxey.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jjgisbdn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mczxhieo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tzbxvpid.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3auxluxag.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxkvoqo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kjttjnog.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ytnrzwjg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jonsmvph.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltnmzkwk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rpwjuncp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ulydcnyo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zqvkawvt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cmqaxqms.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rwbxtuuz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lueffylk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wubbqfcg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hyppprje.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xmzyprwq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xkusuqjw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cdzfwjhv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzmjmxhq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kmrqfpgz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mcqiffyw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewdnfyuo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uoikxwjb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vysjcoml.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jomknzuy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rfyqijrl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zpeghqmb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cajbffgn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3nbmnyrsc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rehaoahk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lihohcxn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3duzydglg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tdqfrkth.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kggkhjio.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vszekmlk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3idemzsrz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rtityqak.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3tfflqnju.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3eqfypcfe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uhmnsiyp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaajblbv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dypyhnor.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijpullwf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dokzkjtb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hohapqem.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qkmjvser.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vadskkqp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3pxaqviiq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qvhdczwu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rekbyndu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wjcrtvrf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjenlfnh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ujgpbyai.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3enhhwqym.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ymczimdc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nvbiycny.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3crbdhfef.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3umvrdhwh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3imyaqnbt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xkftudma.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qlllemxd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lsgmvxof.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nntgoneq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vxrwdxes.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3rrpupnnh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mitlgyzx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vzbpkduu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bmwlqmlj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3prpszgod.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kwbpsqjz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jjfrnzsq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ybrmswnf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yhvqgkeh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jasljkrr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qwrofbwy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvyxwcs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qxjjfoua.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lmyukjxu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ynshbqfd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tbkzedwk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3aaizghht.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ggkwnmex.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tasdhkff.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jlkppypd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkxzyix.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sxsjdoxr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clbulpnj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bowlrgth.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdihtxkn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3djpzwcuq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsiycmb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yldvtkuu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kcntlbqd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hmwqdyhb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dbdbpdki.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sedxixhh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ktqkxhfy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vzcgfdid.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nhtppitn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nbumwjfo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ptfhjzfq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3imwzfukp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpgcmxob.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ycwndpgq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wfxwlaqd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mhwkfhyz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrxmvwm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nquddnjz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ufqkhwkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nslrdpgg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ajemljhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbianhmb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3anxsbivi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uffzsecf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qhgocfeo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thylyfkk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pxevcfxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yejjybjy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mrjjgmcj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mniskxoh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3epikwmpp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jpstouan.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fgpjpnuo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jyyhzcry.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdbkxxkx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvugzghd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tncjmylo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wnjtjwwq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qawlbqlz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3sraqktun.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lqtgkajq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gkgljtfr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxoxhzu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhuehtqt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3metgajjn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vebmhuqn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3srftyyts.html


<!-- 参考信息 -->