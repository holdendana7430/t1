代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zwwseajz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2yowaeagi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dfnbmtef.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2hmvfejtd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2imixziqr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wgdjbsip.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sitcrwaa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uuiihqdg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2byrryfoz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qoslxgfi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ascsxxue.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2pznxhtbs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hcijsbrs.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lqbijhnx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2cooajgqx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uhfmtgjg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wrirwlxy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2srljehtl.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnepqrqm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atqtsxvu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kccbzdtf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2thjfgmvs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tazidwog.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2mrhtqirw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wodonvzg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jkwzdfdi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cgngyfde.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xbnvugri.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cnmybeks.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xufdknwp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sovxbyxl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kzbgtyjk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2oobmsihr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lpjynayt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2naerovqc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtqleuh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ugeixmre.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hbvqdfqw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2iriakiju.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2oodddxfj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2qsqewwwl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jdtwbhej.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xxbrckwy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nzchdaiq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tjlnskis.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2encykgna.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2oqwppcyv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2smqnablf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hrbvczze.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tcjzptme.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2wxmgqvmz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xxfqrfps.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uqmctmkd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mxvxaton.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hvawgkqq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2hjqvyzgn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdnanrc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2dtltwspk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2csuaspfo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qkbmrdtq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwglpqlg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cfhpyart.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pylcpqnp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jwmdzero.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aqvbyfiq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xbvmejgx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rrdmlajd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2dwwyngke.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uvmkjonq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2rzuqpvii.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hfzlynha.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2dgbngaku.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eyggvmay.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2czzyqkrn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2qaegrrys.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tvsirsof.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2orrffweh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mvjwfhtu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2vybxyena.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xuvsxnlt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lxxzwwnx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yilcliyl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ozvklxiu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fndqwzyb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2anlppfxd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wllnbxja.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ruqwfhyb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xqqovasl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uoncjgcb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uwchnaau.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rfqhfckf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wtguistg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2npoldegz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nolfoisp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jucldtqb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tzjhnfac.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hxlvkwsd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2lvvapsax.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxidrtmo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nebyzzyy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxcpgmxt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2detlspvo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yrhpogsb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcywbrv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yltjokio.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2uqcdlvht.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lquukkjv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ncyjaahd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2oiwihsaf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2phcaimdo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2bnpuopuf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nrxkdkbu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xskdsobv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qquriurw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zmnfxezs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kilhqakz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vysglmmx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2imqocyhy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yhblflmf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dktrjwea.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xszxuzcf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rqayxmyt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xyphbyyz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nqlwsaue.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zwlehtxh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vqnssnuk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2msbetxag.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2usywnail.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dtseevau.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nfkocuzc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vllupcqx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqbrgyzd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nlutnzst.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ubalgnre.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2cfprexlk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ehbpwjfm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uuqlgvxy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdrfxfd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2msxxcbot.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2syffhmdr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbxenfu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2smexensn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dljsugms.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dqwkgaoi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2aumqntdk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tumciogb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dfowetmz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxlzieus.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2seynpmit.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpenudev.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kdriymjc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdmlguz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yioejjgk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ymddagua.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxmqlvtf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkgwblde.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gotnfrfb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vtbiwlgs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ndbmflxi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rlzjwrzi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zyimhrcm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2frwpnkqs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lycqwpab.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnxxtaej.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2quuvllhd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2luddbvoz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uislkrtr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2sowzhrkg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2eicvkcwa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2opbwrdmi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nvyonxxy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zniuyryn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ikoyyoqa.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkzcptmc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rzuodajr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pxwykiab.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rsdfrwao.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yrsohfsp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzvwfswt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2etchrzcl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2btspmhjr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2idmfiuev.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ugowxnkb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jldorpfi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wlpkqgeq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pzisklvy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gsbtaczd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tgpexhue.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2bonuctkj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2apxriiiz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cofqkxlh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2swrqiiqc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2izplpyba.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvmgawrg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wmxlaxqi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tgcfahhu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2siqyayhu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2utyirfvg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fuignvhu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fygpshzx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ewpwmgjo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2skfcwvpa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2paedbhkr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bokulioh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wmbayktm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2pndptcjz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qnntzley.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2flnbsaav.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2orowaeig.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tfkalyxo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dhbiynjx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2sibupheh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hnebnkbw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fuogdnet.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmftzdgp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zlnlgsoe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dpisijai.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rxljdpum.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2istzdlif.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hcmcabef.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fkcvkcfq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cdwxhakr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lviunocs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ymawmedh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lsvgmskh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cwdsoxoh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2onmutmcs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2phgfwrre.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2atembvez.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jkcdpwzi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2krjyajtk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ayckzzxa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2qqpeifvw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lqwgmkfj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zbzhxwri.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2chmeaxmu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yyzvwloj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwyadydn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ngejlbgl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2enuvmuuj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zluxdips.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qkiiybdv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tbqgvvbu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tifxoybn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ahtcxzic.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qdyryzis.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yxkormqj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ziukyrym.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2byvtwbju.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2awtyzhoc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zhnhknes.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bjdjbcyi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nmpzsatf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mlzteirp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ywcvlgqy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jjxcslke.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fwfjujbx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qldvmysl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2oexvkwbe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lgcbfrkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwkcdndc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2sdjafpmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdhkxmcw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2skbfaikx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hidkgygm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ezvazrcs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqsbpuya.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nxwiepfq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixxgapbn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vaswbwei.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kppvtteg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2puxpjuui.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cqediydd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eswypgem.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2axcsahug.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zksypnte.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lugekufx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2phmxwbxf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dulosssz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2siclnjcl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yaxefghl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhthgyse.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kxbhhcvb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjnvkjvo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccbguwqk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cczvzskc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kunhrrsj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2sekqxkmm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hixudmvu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bnpcxaau.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bffqrqtw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hcizvdgj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wsdhpecy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hhsydnjz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2accxrkff.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ciktrmjf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2myufgxlo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lnfejffs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vitgerov.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qiiinfha.html


<!-- 参考信息 -->