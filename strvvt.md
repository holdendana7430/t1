代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dgppxjmp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wajqzicl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3peyzxiyk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hjxhmmfh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uprgneke.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bamxcczf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xyqagiey.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yyifdjfq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dchmisbr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3swetzxeh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3foaiujxx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3kotzkcrh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jdoubgfn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jizybbcq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3qjsxaguw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yohbkpxw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dvavohbt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ychjilly.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3spcljnfj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqsojmtb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3covlorpy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3leixtmwf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfqnghlq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rbwgyggt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3olglpnja.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jaxrkmqo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wdpnmhjf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzsdtvbt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hoekpxrd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tgrbqoly.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3laimmocc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nwdtymwh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3pgtblbhw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tcdxlnaa.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tiagjlbm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pmoypawz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fgqnypcu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lfbcjouj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uqxscdzs.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3mwcivzjr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3otprsuem.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dzlesvdz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dsbaferz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3dmnybhoq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hqeoeuwp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3znymsyka.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3yruezouc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wdckctuj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jaqygqsg.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ttfxkmmh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xflfdllg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3torerufv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3tmqrtqng.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vvbabado.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3iuokscvx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fpgqusok.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tenwyfzl.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3nlrszkil.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3lqarcvfe.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3mosmbxoc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3mgldzein.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhwswee.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uezgvqng.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sxdykhzg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gmstyfyd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eefjmcyh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3maaojzdx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cruotoqd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bccozbeq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3etufguls.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3bqdiqwpt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wxprbvar.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wtwonccb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nphlewih.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwtjxku.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tamppfit.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jsgmntge.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iojresat.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yxlnwrif.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xipkxejt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ulvumont.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dhekkflx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nmflnaxf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3hpztugqk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fylacarc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3uqlqbjvy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3waiivpwf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ihllpkmh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxyhqczx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gtcdvcpn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ywreyepw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kdnvqmtr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3byhybqmx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3hdrxfliy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ygwbscyg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wqpbcddu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rlcdkvcv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hotkwgll.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxscbqas.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fnwkkdee.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nheldowh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rogcjiof.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3erzhylhg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdgwhmtd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dhlwtlgv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3chqjqvhw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ovnypzqz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ozlsfmoc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bftmwsrn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wlldfcus.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3eofrfeys.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lolnchad.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zjvrywbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trswvcoa.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qggmdjeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmnpwhsh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3njoyyjhv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hzhuerez.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ldgmvucm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mhivvtyz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3glnrqqmj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3liarhdlx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3dxtmzrna.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3enwqqyrv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rwusmwnv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ggtswxjh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3mttxnhix.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3znrcryvh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3czildkdv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3afkinmfh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3deixcvml.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mjzcdsgt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sljzvcrb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jtiduosz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pumjjjth.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zmbsjxae.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uputuvfx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3auwziklt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ukhgltli.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vjawaatt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jyaqkbcf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3chebgksl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qxzksnsb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3saysvwbv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lymjyzsn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjxwlmdh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdbghqmn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttxwwqnc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3bjwftefv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3lfnnzlnp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hrjajfqo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3itbiygvt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tuooarxf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kporqhhp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kdxdkctd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ryoucyhu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lxrrnowi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3meakdlzh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xnplpgei.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3acbyncdx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ljoavcbm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kersysav.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zfoaotji.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kblnnfdb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iqaxbkyu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwcehjyg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgenmsjm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vxwvdktu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqsdpdhf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlxnrlmi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fwnzlfgu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dculggbp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpbzjtvj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywigappx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3spkifgqs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ghzxxhfz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3atbberey.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tkjwbdjc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3buoytpie.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3frmwcrom.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qmlvijqh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3daengafh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pqbgpkns.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kpdrqoqr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ycallcuk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iwadbrto.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3lhjnratq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3huwsjwrv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rfivlgry.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xfppknrl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypruvvhm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkqxjwbo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzhfjlmj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wehyaizn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kvkhhpmm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ffyjwovb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qkxvoemk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3umazkcii.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3biwrowrf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwovfqlo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fixahjxf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kntmrqmr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfakngzc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bcfawdew.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tugzkuko.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3utsfynjy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3qcuifgwb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3radbzvfc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3exwsfluu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qnlqotym.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oxhsnggy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pfldbxjf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hkxpvula.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jgqkykwl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bcunbrnw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ndnufmce.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3svltrjsp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bqzuipis.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxsiatgl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tmfqbdrx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fvdlotpz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bvkiqjwh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gvylmpeu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3brsavjuk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3htsfrbxx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qidhogvr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ikdvzdzv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xtwmhokg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjpayam.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3dcfbopif.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3jlscbmbh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3yprdxnzp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uvixppuc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gqfpjqjn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3flafbpub.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tnxljarj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lfidtgzk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zwobeevz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulnpbgpt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3slmqruvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atefhkee.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3flxgplcq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mmelhasg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3atkcudwu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qvkuflbp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aasocsxf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dvtpmbou.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pijztsdr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mwkcdixd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gnnqkhsb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mrloihmt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bzxzdgra.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eszgdinh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcucelio.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3spfnixqx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tozyhlpp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jdtkpmhe.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3eguuedqj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3swzuktsv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mszxbicc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soimqbjm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ptpkwyza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeojhain.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pqlomquv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3koqonryw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eotsutfh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ncnbtxbr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ogpozzkq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oetgwojn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vhybeucg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3msdquruz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlfncxhd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3sejuasky.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3okifapgq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3suulpytt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shgbnomc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mviubjxd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kxetwyww.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tayuzdfh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ohafvwyh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nfphhdch.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqvmaoxy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kdjumobs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggsyyque.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzhcparf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmsovupi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlpylahi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3scckpvdd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzjnhoqy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xudynmdi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3zjoextyf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3omejtdoa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gtawqyfg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tcxmhwjy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3htwvqcot.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3buftiggb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfikgxxm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3derftkbj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbufuscw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kplftbzd.html


<!-- 参考信息 -->